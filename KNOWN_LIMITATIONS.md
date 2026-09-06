# Known Limitations — 0.1.0-rc.4

- Phase 1–7 build gates pass with automated regression evidence.
- Phase 8 T0 package validation is build-local; OpenAI, Claude, and Doubao/Feishu T1–T9 remain NOT_RUN until the RC is installed in each target application surface.
- OpenAI Plugin RC is skills-only; the candidate must separately connect/authorize Google Drive. Installation, permission scope and cross-session behavior remain target-runtime TEST_REQUIRED.
- Claude RC includes both canonical `SKILL.md` and application-compatible `skill.md`; actual Customize > Skills upload/activation remains target-runtime TEST_REQUIRED.
- Feishu Bitable Agent is the provisional first Doubao/Feishu test surface; tenant/product availability and exact upload/publish behavior remain TEST_REQUIRED.
- Channel endpoints can change; access failure must continue to be recorded as a Channel Gap rather than zero supply.
- Scheduler, retry, run-history, notification, and stop behavior remain target-runtime TEST_REQUIRED.
- Authenticated browsing and per-channel terms/account-risk boundaries remain TEST_REQUIRED and are never default capabilities.
- GitHub public/private repositories are the distribution and development control plane. Binary Release-asset publication is still a distribution operation and must preserve version/checksum parity.
- The Public Beta is source-available under an evaluation/testing license, not an open-source license; redistribution and commercial derivative distribution are not granted.
- Public Beta is allowed before all three target-runtime tests are complete, provided unverified capabilities are explicitly labeled TEST_REQUIRED / Experimental. Stable `v0.1.0` remains prohibited until three-surface T1–T9, semantic parity, release review, and Go/No-Go pass.
