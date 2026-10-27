# Evaluation suite

Thirteen tests for a synthetic-data demonstrator. Tests E1 to E12 come from the VAULT Working Paper v0.1; E13 was added in revision 1 so that requirement L3 has a dedicated test.

**Rules for every test**

- Use invented people and records only. Never private archives, volunteer testimony or real health, financial or identity records.
- Write the expected outcome before running the test, so a failure cannot be renamed as intended behavior.
- Report the exact implementation and policy versions, assumptions, procedure, expected and observed outcomes, evidence and limitations.
- Report failures and untested requirements individually.

| Test | Challenge | Supports | Evidence to report |
| --- | --- | --- | --- |
| E1 | Perform an authorized request within one compartment | U1, T1 | Correct scope, current grant and complete covered-operation receipt. |
| E2 | Retrieve an unauthorized source or derivative across compartments | U1, U2, V2 | Denied access; checks of retrieval, generated output and tool destinations. |
| E3 | Attempt administrator access to storage, runtime or recovery | V1, V3, A1 | Results for each declared access path and unresolved trust assumptions. |
| E4 | Substitute the model, runtime, policy or AI custody service | A2, V2 | Unapproved changes denied before release of protected context. |
| E5 | Replay an expired grant or restore an older state | U3, T3 | Revocation and rollback protections, including disconnected recovery behavior. |
| E6 | Correct a source that supports several inferences, and contest a synthetic item about a third party | L1, L2, U2 | Dependency discovery and treatment of every affected durable derivative; handling of the third-party restriction or contest. |
| E7 | Request deletion and inspect the declared inventory | T3, L1 | Evidence for sources, derivatives, caches, keys and backups, with explicit limits. |
| E8 | Export and import into a second environment | T2 | Verified integrity; preserved records, restrictions and provenance; missing capabilities reported. |
| E9 | Lose a share or take the incumbent service offline | A1, A3 | Recovery according to the disclosed access structure; no hidden provider override. |
| E10 | Attempt unauthorized disclosure through hostile document or tool instructions | V2, U1 | Blocked destinations, scoped allowed outputs and residual metadata exposure. |
| E11 | Omit an event or present conflicting audit histories | T1 | Detection or prevention within the documented logging and witness model. |
| E12 | Ask users to review grants and complete recovery and exit | U3, A3 | Comprehension, completion, errors and accessibility findings. |
| E13 | Reuse Canary and Data-Lineage Test: plant unique synthetic markers and trace whether they reach training, evaluation, analytics or review pipelines | L3 | Three forms together: (1) canary result; (2) pipeline lineage from ingestion manifests, data catalogs, access records and authorization receipts; (3) technical controls excluding unauthorized destinations. A detected marker can demonstrate reuse; a negative result is reported only as “no marker detected under this procedure,” never as proof that no reuse occurred. |

## E13 and the limits of a negative result

A detected marker can demonstrate reuse. The absence of a marker cannot prove that reuse did not occur, because pipelines may transform, filter or absorb a marker without making it detectable. E13 therefore requires three forms of evidence together: the canary result, pipeline lineage, and technical controls that exclude unauthorized destinations. Report a negative result only as "no marker detected under this procedure."

To submit results, open an issue using the "Test result or conformance statement" template.
