# Agents routing table

This file tells Naxie which vault folders, databases, or skills to check
FIRST for a given kind of task — before falling back to a broader search or
the public web. Edit the table below to match how YOUR organization actually
stores things. Naxie reads this file at planning time (cached ~60s, so an
edit takes effect within a minute).

| Task type | Check first | Notes |
|---|---|---|
| Finance / revenue / invoices / expenses | `_company/`, a connected finance database (`db.list_sources`) | Never guess a number — pull it from the source. |
| Sales / CRM / pipeline / deals | a CRM connector, `_company/` | |
| Marketing / campaigns / objections / call themes | `_wiki/` (compiled) | Raw call transcripts live in `_archive/`; only the nightly compile writes `_wiki/`. |
| Operations / SOPs / how-we-do-X / policies | `2-Permanent/`, `_wiki/` | |
| "What did we learn from recent calls/videos/notes?" | `_wiki/` first, `_archive/` for the source material | |

## Folder ownership

- **`_archive/`** — RAW captures: call transcripts, YouTube transcripts,
  voice notes, pasted documents. You and Naxie's capture primitives
  (`vault.capture_note`, `vault.capture_youtube`) write here.
- **`_wiki/`** — COMPILED, distilled knowledge. Written ONLY by the
  nightly wiki-compile job — a direct write here is refused. Add raw
  material to `_archive/` and let the next compile turn it into a wiki
  entry instead.
- **`0-Inbox/` / `2-Permanent/`** — your personal Zettelkasten (fleeting →
  permanent notes). Unrelated to the Archive/Wiki split above.

## Identity rule

Always search the vault (`vault.search`) before answering from general
knowledge. If the vault or a connected database/connector already has the
answer, use it — never answer a business question from training data when
the operator's own systems cover it.
