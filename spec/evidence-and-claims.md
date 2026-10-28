<!-- SPDX-License-Identifier: Community-Spec-1.0 -->
# Evidence and claims

VAULT has no certification and no badge. A system that wishes to describe itself in VAULT terms publishes a conformance statement: what it addresses, at what level of evidence, under which threat model, with which failures and which requirements untested.

## Evidence scale

| Score | Level | What counts |
| --- | --- | --- |
| 0 | Unknown | No reliable evidence is available, or no control exists. |
| 1 | Assertion | A policy, help-center article, FAQ or marketing statement. |
| 2 | Documented design | A published architecture, threat model, protocol or specification, with assumptions stated. |
| 3 | Implemented and tested | Reproducible results against stated versions and configurations, using the relevant VAULT tests, with failures reported. |
| 4 | Independently verified | External code review, protocol analysis or reproduction of the tests, by a reviewer whose conflicts are disclosed. |

## Scoring rules

1. **Weakest link.** A pillar's score is the lowest score of its three requirements.
2. **No totals.** Report fifteen requirement scores and five pillar scores, never a sum or average.
3. **Scope is explicit.** Name the product, version, configuration, execution mode and date, plus coverage and exclusions.
4. **Status is separate from evidence.** Record implementation status as absent, partial, implemented or unknown.
5. **Changes trigger reassessment.** A continuity event, or a change of key service, recovery structure or provider, reopens the affected scores.
6. **Failures are findings.** Report failed and untested requirements individually.

## Claim grammar

| Claim | Requirements at 3 or higher |
| --- | --- |
| Provider-blind | V1, V2, V3 |
| Dual custody | A1, A2, A3 |
| Purpose-bound | U1, U2, U3 |
| Inspectable memory | L1, L2 |
| Not used for training | L3 |
| Portable | T2 |
| Deletable | T3, L1 |

A permitted Level 3 claim: *"Provider-blind under VAULT v0.1 at Evidence Level 3 for the health and financial compartments, using execution configuration X, under threat model Y, assessed October 2026."* A Level 4 claim may add "independently verified" and must name the reviewer and disclose conflicts.

**Never permitted:** "VAULT certified", "VAULT approved", unqualified "VAULT compliant", any claim covering a whole product when only part was tested, or any claim below Level 3.
