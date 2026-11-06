# Tests

**No executable test suite exists yet.** This folder reserves the verification workstream and records the plan.

| Layer | Planned coverage |
| --- | --- |
| Detector unit tests | Known complex vectors, noise-only and signal-present cases, threshold boundary, normalization and invalid inputs |
| Simulation regression | Reproduce archived GNU Radio baseline with recorded settings and tolerances |
| Receiver / RF | Opt-in hardware acquisition and labeled RF trials; never run implicitly |
| Cooperative sensing | Fusion decisions, missing/stale/duplicate reports and clock assumptions |
| Blockchain | Access control, valid/invalid submissions, retries and receipt verification |
| End-to-end | Trace observation and decision to its ledger evidence |

Add a documented test command and tested dependency versions when executable tests are introduced. Do not report this plan as a passing test suite. See [validation](../documentation/VALIDATION.md).
