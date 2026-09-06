# Beta Status — 0.1.0-rc.4

## Build gate
PASS.

- 21 canonical schemas validate.
- Negative semantic constraints pass.
- Three adapters round-trip the canonical fixture without critical semantic drift.
- 40-item Ground Truth v0.2 validates with evidence/time/status/degradation semantics.
- Monitoring regression: official-first 40/40; trusted-origin P0/P1 100%; closed false-open 0; controlled dedup 100%; access-failure zero-supply inference 0.
- Learning regression: scoped trials and rollback pass; cross-scope pollution 0.
- Prompt/recovery regression: support/login/suppression/no-auto-send gates pass.
- RC4 package T0 validation passes for Core, OpenAI, Claude and Doubao+Feishu.
- Active tree, distributable packages and rewritten Git history contain no deprecated private support email.

## Runtime validation
OpenAI / Claude / Doubao+Feishu T1–T9 is being collected during Public Beta. Unsupported or unverified runtime claims remain TEST_REQUIRED.
