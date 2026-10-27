# VAULT specification

The fifteen requirements, one file per pillar. Requirement IDs are stable: refer to them (for example, "A2") in issues and proposals.

| ID | Requirement | Minimum outcome |
| --- | --- | --- |
| [V1](V-verifiable-provider-blindness.md) | No independent provider access | No provider-exercisable key, console, recovery route or side path reveals protected plaintext. Any such route, whatever it is called, fails V1; disclosure does not cure it. |
| [V2](V-verifiable-provider-blindness.md) | Approved execution and egress | Context reaches only a freshly verified boundary, and cannot leave it or reach an unauthorized recipient through logs, telemetry, tool calls, generated outputs, fallbacks or any other egress route. |
| [V3](V-verifiable-provider-blindness.md) | Independently assessable evidence | Threat model, trusted computing base, collusion sets, update authority, residual metadata exposure and known failures are public and reviewable without private data. |
| [A1](A-ai-user-dual-custody.md) | Separate authorization domains | Two separately held, individually insufficient authorities are required; the provider independently controls neither, and the protocol states where plaintext and short-lived keys exist. |
| [A2](A-ai-user-dual-custody.md) | Bind authority to identity and change control | A changed model, runtime or policy reaches existing context only through a documented, authorized transition naming it a continuation, successor, fork or new participant; nothing inherits authority silently. |
| [A3](A-ai-user-dual-custody.md) | Preserve access without captivity | The person can always retrieve their own records independently; dual custody governs managed access, never captivity. |
| [U1](U-purpose-and-compartments.md) | Narrow authorization | Every grant names its compartments, operations, recipients, tools, duration and execution identity, enforced in code. |
| [U2](U-purpose-and-compartments.md) | Restrictions follow information | Derivatives carry their sources' restrictions; combined material carries the combined restrictions; reductions are explicit and recorded. |
| [U3](U-purpose-and-compartments.md) | Understandable continuing consent | Active access is visible and closable; grants expire or are reviewed; material changes are shown side by side before they apply. |
| [L1](L-locked-source-and-derived-intelligence.md) | An inventory with provenance | Every retained source and derivative is inventoried with provenance, and the inventory is protected like the content. |
| [L2](L-locked-source-and-derived-intelligence.md) | Inspect and correct the portrait | People can read what is durably held about them, see what is stated, inferred or disputed, and correct it with effect on dependent derivatives; third-party information can be restricted, contested and deleted. |
| [L3](L-locked-source-and-derived-intelligence.md) | Govern every reuse | No training, analytics, advertising or human review without specific authorization; adaptations are in scope; unremovable influence is disclosed in advance. |
| [T1](T-transparency-transfer-termination.md) | Protected and verifiable receipts | Every covered operation produces a private, integrity-protected receipt, and omissions or conflicting histories can be detected. |
| [T2](T-transparency-transfer-termination.md) | Functional transfer | Export is an authenticated, documented package, proven by import into a second environment, with missing dependencies and behavior changes reported. |
| [T3](T-transparency-transfer-termination.md) | Scoped termination | Revocation works within a declared delay; deletion reports scope, timing and exceptions across sources, derivatives, keys, backups and caches. |

Also in this folder: [key terms](key-terms.md) and [evidence and claims](evidence-and-claims.md).
