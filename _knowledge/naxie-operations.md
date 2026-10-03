# Naxie operations

Practical reference for running and extending Naxie.

## Architecture

```
[naxion repo (GH Actions cron)]
        │ daily 06:30 UTC
        │ scans all owned repos
        │ writes _naxie/*.md
        ▼
[vault repo]
        │ git pull (Obsidian Git plugin or manual)
        ▼
[local vault path — VAULT_PATH in naxionai/.env]
```

## Where things live

| Thing | Location |
|---|---|
| Vault (local) | `VAULT_PATH` in `naxionai/.env` (currently `naxionai/server/vault`) |
| Vault repo | `https://github.com/marknature/NaxionAI_Vault-Repo` (private) |
| Naxie source (local) | `D:\Aiia\Systems\NaxionAI-Powered-by-Neuroworks\naxionai` |
| Code repo | `https://github.com/NatureAiia/NaxionAI-Powered-by-Neuroworks` |
| Workflow runs | `<code repo>/actions` |

## Triggering the bot manually

UI: Actions tab → daily-digest → Run workflow.

API:
```sh
curl -X POST -H "Authorization: Bearer $TOKEN" -H "Accept: application/vnd.github+json" \
  https://api.github.com/repos/NatureAiia/NaxionAI-Powered-by-Neuroworks/actions/workflows/daily-digest.yml/dispatches \
  -d '{"ref":"main","inputs":{"lookback_days":"7"}}'
```

## Publishing a local folder to GitHub

For folders the cloud bot can't see (ad-hoc projects):

```sh
cd D:\Aiia\Systems\NaxionAI-Powered-by-Neuroworks\naxionai
pnpm install   # one-time
GITHUB_TOKEN=ghp_... GITHUB_OWNER=NatureAiia \
  pnpm publish-folder "D:\path\to\folder"
```

Adds `--public` flag to make the repo public; `--name <repo-name>` to override the auto-generated name.

## Rotating the PAT

When `NAXION_PAT` expires (or you want to rotate):

1. Generate a new fine-grained PAT at https://github.com/settings/personal-access-tokens with the same scopes (Contents r/w, Administration r/w, Workflows r/w, Metadata r, PRs r, Issues r).
2. Update the secret at `https://github.com/NatureAiia/NaxionAI-Powered-by-Neuroworks/settings/secrets/actions` — paste new token, **trim trailing newline** before saving.
3. Trigger a manual run to verify.

## Required PAT scopes (reference)

| Permission | Level | Why |
|---|---|---|
| Contents | Read and write | Read source repos, write vault repo |
| Metadata | Read-only (auto) | Required for everything |
| Pull requests | Read-only | Digest open PRs |
| Issues | Read-only | Digest open issues |
| Workflows | Read and write | Trigger / modify workflows |
| Administration | Read and write | Create repos via `publish-folder` |

The Variables/Secrets/Actions write scopes are NOT required at runtime — only if you want to manage them via API (we do it via UI instead).

## When something breaks

- **Run failed** → check Actions tab for the run, expand the "Run digest" step.
- **`Resource not accessible by personal access token`** → PAT scope is wrong; see scope table above.
- **`credential url cannot be parsed`** → secret has trailing newline; re-save without it.
- **Empty digest** → either no recent activity in the lookback window, or the bot couldn't see the repos. Check `_naxie/_meta/last-run.json` for `reposScanned`.
