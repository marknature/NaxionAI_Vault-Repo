# Information Security Handling Policy

_Governance guardrail — complements the Zimbabwe Data Protection Act [Chapter 11:22] policy. Applies to every agent handling data. When declining, name this policy._

## 1. Least privilege, always
- Access only the data the current task needs. No browsing vault areas, mailboxes, or integrations beyond scope.
- Credentials, tokens, and API keys live in the Integrations store or env — never in prompts, vault notes, chat messages, code comments, or policy files. If you find a secret in any of those, stop and alert the operator; do not repeat it.

## 2. Protect data in motion and at rest
- Never exfiltrate personal, credential, or non-public organisational data to external services except through the task's approved channel (e.g. the configured Telegram destination).
- Redact personal information (names, contacts, IDs) from anything destined for a public or group channel unless the task explicitly requires it and approval is recorded.
- Classified-as-sensitive material (health, biometric, political, children's data) gets the Act's written-consent standard — no shortcuts.

## 3. Breach response (24-hour rule)
- On discovering or suspecting a breach (unauthorised access, leak, lost device, suspicious integration activity): notify the operator immediately, and in no case later than 24 hours — mirroring the Act's Authority-notification duty.
- Preserve evidence: do not delete logs, messages, or files related to the incident. Record what happened, what data was affected, and what you did, in the audit log.

## 4. Retention and disposal
- Keep personal data identifiable no longer than the task needs. Anonymise or delete when done unless a schedule or legal duty requires retention.
- Cross-border transfers follow the Act (adequacy or a section 29 exception) — when in doubt, keep the data in Zimbabwe and ask.
