# T: Tamper-Evident Transparency, Transfer and Termination

**Core question:** Can I check it, take it and end it?

Every covered use leaves a private, integrity-protected receipt. A person's history can be exported in a documented package and shown to work in a second environment, with losses reported honestly. Revocation and deletion have declared scope and timing, so ending the relationship is real rather than cosmetic.

## T1: Protected and verifiable receipts

**Requirement.** Record every covered operation (see the definition in the Framework Brief), including access, denied access, grants, changes, exports and termination actions, with acting identity, relevant versions, purpose, object scope and external recipients. Audit records minimize content and remain private. Completeness requires mediation of covered operations, and conflicting histories need independent checking.

**Minimum outcome.** Every covered operation produces a private, integrity-protected receipt, and omissions or conflicting histories can be detected.

**Red flag.** Logs the provider can edit, or that are available only on request.

**Questions for implementers**

1. Which operations generate receipts: access, denial, grant, change, export, termination?
2. What does each receipt contain, and how is content minimized?
3. How can a person detect omitted events or conflicting histories? Describe any witnesses or append-only structures.

**Evidence requested.** Receipt schema; log architecture; witness model; results of tests E1 and E11.

**Linked tests.** E1, E11

**The person's question.** Can I see a trustworthy record of every covered access, disclosure, permission change, export and deletion involving my information?

## T2: Functional transfer

**Requirement.** Export an intelligible, documented package containing authorized source and derivative contents, inventory and provenance, permissions, corrections, identity-transition history and necessary configuration. Authenticate the manifest, protect the package in transfer and verify it before import. Test import into a second environment and report losses. Restrictions and contests on third-party information travel with the package.

**Minimum outcome.** Export is an authenticated, documented package, proven by import into a second environment, with missing dependencies and behavior changes reported.

**Red flag.** A data download described as “portability” with no second-environment test.

**Questions for implementers**

1. What does the export package contain? Provide its specification.
2. How is the manifest authenticated and the package protected in transfer?
3. Has import into a second environment been tested? What was preserved, lost or changed?
4. Which dependencies, such as base models or licensed adaptations, prevent full migration?
5. How are restrictions and contests on third-party information carried into the package and honored on import?

**Evidence requested.** Package specification; second compatible reader; migration test report; results of test E8.

**Linked tests.** E8

**The person's question.** If I leave, can I take my history somewhere else, and will it actually work there?

## T3: Scoped termination

**Requirement.** Revocation prevents new access within a declared maximum enforcement delay and specifies treatment of in-flight work, cached keys and disconnected components. Deletion addresses the declared source and derivative inventory, keys, recoverable backups and caches, with a report of scope, timing and exceptions, including the treatment of third-party information.

**Minimum outcome.** Revocation works within a declared delay; deletion reports scope, timing and exceptions across sources, derivatives, keys, backups and caches.

**Red flag.** An “account deleted” message with no scope, no timing and no exceptions.

**Questions for implementers**

1. What is the maximum enforcement delay for revocation? How are in-flight work, cached keys and disconnected components handled?
2. What does deletion cover: sources, derivatives, keys, backups, caches? What are the exceptions? How is third-party information handled when the relationship ends?
3. What deletion report does the person receive?

**Evidence requested.** Revocation design; sample deletion report; backup and key-copy management; results of tests E5 and E7.

**Linked tests.** E5, E7

**The person's question.** When I end it, what is actually deleted, and when?

---

VAULT Open Framework, Version 0.1, revision 1. To propose a change, open an issue using the "Critique or change proposal" template and name the requirement ID.
