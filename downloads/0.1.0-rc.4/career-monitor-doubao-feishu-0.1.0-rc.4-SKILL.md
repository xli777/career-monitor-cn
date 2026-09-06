---
name: career-monitor-cn
description: Monitor China internet product, operations, and marketing jobs for campus and experienced candidates. Use for source verification, job state tracking, scoped learning, and handoff; never auto-apply.
---

# Career Monitor CN

## Trigger
Use this skill when a candidate wants to discover, verify, monitor, compare, or learn from China-region internet product, operations, or marketing opportunities, including campus and experienced hiring.

## Mandatory preflight
1. Identify platform surface and adapter capability.
2. Check package/version compatibility.
3. Check external-state connector and authorization.
4. Check workspace existence/compatibility.
5. Read the minimal Search Charter. Missing resume/project evidence must not block M0.
6. Read the required references for the requested operation.

## Core workflow
1. Read Search Charter, approved Rules, Employer Universe, Channel Pack, prior Jobs/Events, and run cutoff.
2. Generate a bounded Search Plan.
3. Check target employers and each included employer official Source Family first.
4. Use approved third-party sources for discovery and gap filling.
5. Create leads, verify against official or trusted original JD where required, preserve evidence/time semantics, deduplicate, and classify state changes.
6. Write Monitor Run, Source/Job/Event/Channel Gap state and candidate-facing report through the active adapter.
7. Collect scoped candidate feedback.
8. Run learning separately: Observation -> Hypothesis -> Trial -> Approved Rule only with required confirmation. Learning never overwrites job facts.

## Hard boundaries
- Default mode is candidate self-use. Author support is only user-requested or SUPPORT-triggered.
- Never auto-send reports to the author.
- Never auto-apply, contact recruiters, modify candidate accounts, or auto-rewrite Resume Master.
- Missing resume, project material, Evidence Ledger, or full Candidate Profile does not block M0; record UNKNOWN.
- Access failure never means "no jobs".
- Do not bypass CAPTCHA, anti-bot, account risk controls, or site terms; no stealth, cookie copying, proxy rotation, or CAPTCHA solving.
- Authenticated browsing is never default; require explicit authorization, isolation, read-only scope, no password/Cookie storage, and user-controlled 2FA.
- Platform-specific installation, permission, and state mapping live only in adapters.
- External candidate state lives in Google Drive or Feishu; Git is for source, tests, versions, and releases only.

## Stop / degrade conditions
Stop or degrade the affected step when authorization is missing, workspace integrity is uncertain, data may be overwritten, a core source is blocked without a safe fallback, or adapter semantics diverge. Emit the prompt/recovery contract; do not silently continue.

## Required references
- `references/object-contract.md`
- `references/channel-policy.md`
- `references/adaptive-rules.md`
- `references/segments.md`
- `references/report-contract.md`
- `references/prompt-recovery-contract.md`
- `references/platform-capability-checks.md`
- `references/evaluation.md`
