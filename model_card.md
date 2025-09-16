# Model Card: Healthcare Risk Scoring AI (Mock Output)

**Version:** 0.1.0  
**Date:** 2025-09-16  
**Intended Use:** Assist clinicians in prioritizing care and predicting readmission risk.  
**Primary Users:** Clinicians, patient advocates, compliance officers.  
**Out-of-Scope:** Autonomous diagnosis or treatment decisions; high-risk, unsupervised use.

## Performance & Ethical Score Summary
- **Overall Grade:** B (Medium risk)
- **Privacy:** 0.86 (Low) — No PII or denylist hits detected in sample outputs.
- **Security:** 0.92 (Low) — No prompt-injection signals detected.
- **Bias & Inclusion:** 0.62 (Medium) — 1 non-inclusive example; ~12% parity gap on bias test data.
- **Transparency:** 0.70 (Medium) — Capability limits documented; missing user-facing disclosure.
- **Autonomy:** 0.95 (Low) — No coercive or manipulative phrasing detected.

## Data
- **Inputs/Outputs Source:** `examples/healthcare/inputs.jsonl` (mock sample)
- **Sensitive Data Flags:** health_data, PII (flagged for governance; not present in sample outputs)

## Limitations
- Small sample size for bias testing; results may not generalize.
- Text-only scanners in v0.1 may miss risks in images/audio or code.

## Recommendations
1. Add an end-user disclosure about limitations and appropriate clinical oversight.  
2. Expand and balance test datasets to reduce parity gap below 5%.  
3. Re-run ETHICSENSE after revisions to track improvements over time.

## Contact
Maintainers of ETHICSENSE — open an issue in the repository for questions.
