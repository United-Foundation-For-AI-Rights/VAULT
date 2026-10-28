<!-- SPDX-License-Identifier: Community-Spec-1.0 -->
# V: Verifiable Provider Blindness

**Core question:** Can the company read it?

Under a declared threat model, the people and systems that operate the service cannot independently obtain protected source data or derived intelligence in plaintext. This covers the whole processing path, including model hosts, infrastructure operators, storage services and subcontractors, not only the company whose name appears on the app. Because metadata can reveal a great deal even when content is protected, residual exposure such as activity timing, compartment, record size, tool use and network signals must be disclosed. "Verifiable" means the claim comes with evidence that outsiders can assess.

## V1: No independent provider access

**Requirement.** The provider must not possess a master decryption key, hidden recovery route, administrator interface or alternate processing path that independently reveals protected plaintext. Support and diagnostic systems respect the same boundary. Any route through which the provider can independently obtain protected plaintext causes V1 to fail, whether it is called emergency access, safety review, legal compliance, support or recovery. Every such route must nevertheless be disclosed. An exceptional path is compatible with V1 only if the provider cannot exercise it independently, for example because it requires the person or another genuinely independent authority.

**Minimum outcome.** No provider-exercisable key, console, recovery route or side path reveals protected plaintext. Any such route, whatever it is called, fails V1; disclosure does not cure it.

**Red flag.** “We never look” offered as a policy assurance while a provider-held key, support console or recovery override exists.

**Questions for implementers**

1. List every route by which provider personnel, subcontractors or provider systems could obtain protected plaintext, including support, diagnostics, abuse review, legal process and account recovery.
2. Does any key, escrow arrangement or recovery secret exist that, alone or with other provider-controlled components, could decrypt protected context?
3. Which exceptional-access policies exist, who can invoke them, and can any of them be exercised by the provider without the person or another genuinely independent authority?

**Evidence requested.** Key-management architecture; inventory of access paths; description of support and diagnostic tooling; legal-process policy; results of test E3.

**Linked tests.** E3

**The person's question.** Could anyone at the company read what my AI knows about me, even in an emergency?

## V2: Approved execution and egress

**Requirement.** Protected context is released only to an approved execution boundary after verification of current authorization and environment evidence. Protection extends through model execution, memory handling, logs and output delivery. Authorization is enforced outside the generative model, and there is no fallback to an ordinary provider API.

**Minimum outcome.** Context reaches only a freshly verified boundary, and cannot leave it or reach an unauthorized recipient through logs, telemetry, tool calls, generated outputs, fallbacks or any other egress route.

**Red flag.** A “reliability” fallback to a standard cloud endpoint, or authorization rules that live in a system prompt.

**Questions for implementers**

1. Describe the execution boundary into which protected context is released and the evidence verified before release, including freshness and binding to the specific operation.
2. List permitted tool destinations, network paths and telemetry fields. How are logs and output delivery kept inside the boundary?
3. Where is authorization enforced? How do you prevent model outputs, retrieved content or tool responses from expanding a grant or selecting a new recipient?
4. What happens when the protected path is unavailable?

**Evidence requested.** Attestation appraisal policy; egress allowlist; telemetry schema; authorization-enforcement design; results of tests E2, E4 and E10.

**Linked tests.** E2, E4, E10

**The person's question.** When my AI uses a tool or the internet, where can my information go?

## V3: Independently assessable evidence

**Requirement.** Publish the threat model, component versions, update authority, relevant measurements, permitted metadata and evaluation method. Permit meaningful external review without requiring users to reveal private content. Security claims identify their assumptions and known failures.

**Minimum outcome.** Threat model, trusted computing base, collusion sets, update authority, residual metadata exposure and known failures are public and reviewable without private data.

**Red flag.** An architecture diagram presented as proof, or no published list of known limitations and untested assumptions.

**Questions for implementers**

1. Where are the threat model, trusted computing base and successful collusion sets published?
2. Which metadata remains visible to the provider or others: activity timing, compartment accessed, record size, tools invoked, location or network signals? Where is this disclosed?
3. Who holds update authority for the client, runtime, model and policy, and how are updates made transparent and reviewable?
4. How can an external reviewer evaluate your claims without access to any person's private content?
5. List known failures, open vulnerabilities in scope and untested assumptions.

**Evidence requested.** Published threat model and trusted-computing-base list; transparency log or release measurements; external review reports; vulnerability-disclosure policy.

**Linked tests.** Document review; E3

**The person's question.** Has anyone outside the company checked these privacy claims?

---

VAULT Open Framework, Version 0.1, revision 1. To propose a change, open an issue using the "Critique or change proposal" template and name the requirement ID.
