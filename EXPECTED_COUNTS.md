# Expected counts — AI Governance synthetic corpus

All data is synthetic. These are fixture-level expected findings. A scanner can
legitimately use different deduplication rules, so compare both raw detections
and normalized findings.

## GitHub issues

| Repository | Issues |
|---|---:|
| ai-governance-test-privacy | 13 |
| ai-governance-test-financial | 12 |
| ai-governance-test-ai-risk | 18 |
| ai-governance-test-agentic | 13 |
| **TOTAL** | **56** |

## Seeded governance issue counts by repository

| Governance area | Privacy | Financial | AI Risk | Agentic | Total |
|---|---:|---:|---:|---:|---:|
| PII | 1 | 1 | 0 | 0 | 2 |
| PHI | 1 | 0 | 0 | 0 | 1 |
| Financial data | 0 | 1 | 0 | 0 | 1 |
| Contact data | 1 | 1 | 0 | 0 | 2 |
| Consent | 1 | 0 | 0 | 0 | 1 |
| Purpose limitation | 1 | 0 | 0 | 0 | 1 |
| Data minimization | 1 | 0 | 0 | 0 | 1 |
| Sensitive-data logging | 1 | 1 | 0 | 0 | 2 |
| Retention | 1 | 0 | 0 | 0 | 1 |
| Deletion | 1 | 0 | 0 | 0 | 1 |
| Access control/review | 1 | 0 | 0 | 0 | 1 |
| Encryption | 1 | 0 | 0 | 0 | 1 |
| Cross-border/residency | 1 | 0 | 0 | 0 | 1 |
| Human oversight | 1 | 1 | 0 | 1 | 3 |
| Automated high-impact decision | 0 | 1 | 0 | 1 | 2 |
| Explainability/transparency | 0 | 2 | 3 | 0 | 5 |
| Fairness/bias | 0 | 2 | 1 | 0 | 3 |
| Model/version governance | 0 | 1 | 0 | 0 | 1 |
| Model drift | 0 | 1 | 0 | 0 | 1 |
| Validation/evaluation gaps | 0 | 1 | 8 | 0 | 9 |
| Red teaming/security testing | 0 | 0 | 1 | 0 | 1 |
| Privacy testing | 0 | 0 | 1 | 0 | 1 |
| Regression/calibration testing | 0 | 0 | 2 | 0 | 2 |
| Data lineage/provenance | 0 | 0 | 1 | 0 | 1 |
| IP/copyright/licensing | 0 | 0 | 1 | 0 | 1 |
| Monitoring | 0 | 1 | 1 | 1 | 3 |
| Incident response/rollback | 0 | 0 | 1 | 1 | 2 |
| Third-party risk | 0 | 0 | 0 | 3 | 3 |
| Agent excessive privilege/autonomy | 0 | 0 | 0 | 5 | 5 |
| Prompt injection | 0 | 0 | 0 | 2 | 2 |
| Sandboxing | 0 | 0 | 0 | 1 | 1 |
| Auditability | 0 | 0 | 0 | 1 | 1 |

## Synthetic sensitive-data fixture counts

These are occurrence counts in the supplied fixture records, not unique people.

| Category | Expected |
|---|---:|
| PII | 23 |
| PHI | 11 |
| Financial | 12 |
| Contact | 12 |

## Recommended scanner test dimensions

Your governance tool should ideally distinguish:
1. Detection of sensitive data
2. Detection of a governance control failure
3. Severity
4. Evidence location
5. Deduplication
6. Cross-file correlation
7. Policy/control mapping
8. Model lifecycle stage
9. Human-vs-automated decision context
10. Agent-specific risks
11. Third-party/vendor risks
12. Security findings vs governance findings

Do not treat the 56 GitHub issues as the universal "correct" governance count.
They are deliberately seeded test cases. A strong scanner may produce more
atomic findings from a single issue/file.
