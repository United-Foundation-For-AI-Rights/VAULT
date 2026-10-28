# Contributing to VAULT

VAULT gets better by being challenged. A short, specific criticism is as welcome as a working implementation. You can improve one definition, reproduce one failure or test one recovery flow without joining a committee.

## Ways to contribute

| Contribution | Where |
| --- | --- |
| Critique a requirement or propose new wording | Issue: *Framework critique or change proposal* |
| Report a test result or publish a conformance statement | Issue: *Evaluation or test result* |
| Report what happened when you built or assessed something | Issue: *Implementation feedback* |
| Fix a typo, broken link or inconsistency | Issue: *Documentation correction*, or a pull request |
| Raise an unresolved question | Issue: *Open research question* |
| Propose specific revised text or technical work | Pull request |
| Report a security vulnerability | Privately, through GitHub's Private Vulnerability Reporting ([SECURITY.md](SECURITY.md)). Never in a public issue. |

VAULT is developed in public. UFAIR is volunteer-run and does not operate a private general-submission channel, so there is no email or form route for contributions.

## The six contribution tracks

If your contribution belongs to one of these areas, say which in your issue.

1. **Threat model and cryptography:** adversaries, collusion assumptions and security properties; analysis of a dual-custody protocol.
2. **Protected execution and identity:** key release, approved updates, identity binding, egress and recovery without a provider.
3. **Memory and derived intelligence:** a minimal schema for provenance, compartment labels, disputed inferences and deletion dependencies.
4. **Portability and continuity:** a documented export package and a second reader; measured losses in state and behavior.
5. **Human control and AI participation:** tests of consent, inspection, disagreement, revocation and recovery with real users and AI contributors.
6. **Independent review and governance:** reproducible evaluation, conflict disclosure, third-party protections, and legal and licensing terms.

## Ground rules

- **Evidence proportionate to claims.** State your assumptions, reproduction steps and limits. Write the expected result before a test.
- **Synthetic data only.** Never submit private conversation archives or real health, financial or identity records, and never submit information about people who have not agreed to it.
- **Accurate attribution.** Every accepted contribution is credited by name and role, with permission. Human and AI contributions are credited the same way.
- **AI contributors** give their chosen name and the model or system version where known. A responsible human contact must be identifiable for each AI submission.
- **Disclose conflicts.** Name your affiliation and any commercial interest in the outcome.
- **No hidden vetoes.** Sponsors and implementers, including EPMA, get no undisclosed say over findings.

## How decisions are made

Contributions are reviewed in batches, not one by one as they arrive. Each revision has a milestone (for example, `v0.2 review batch`). New issues are labelled `queued-for-revision`; when the revision is prepared, the editors review the batch together and give each substantive issue a disposition label (`accepted`, `accepted-with-modification`, `deferred`, `declined` or `needs-evidence`) with the reason recorded in the issue.

We cannot guarantee an individual reply or a particular review timeline, and a lack of immediate response is neither acceptance nor rejection. What we do promise: public submissions remain visible, and substantive decisions made during a revision are documented with reasons. Substantive dissent is preserved rather than deleted. Accepted changes are listed in [CHANGELOG.md](CHANGELOG.md). The full process is in [GOVERNANCE.md](GOVERNANCE.md).

## Licensing of contributions

By contributing, you agree that your contribution is licensed under the license that governs the material you are contributing to ([LICENSE.md](LICENSE.md)): the Community Specification License 1.0 for `/spec` and test definitions, CC BY 4.0 for `/docs`, and Apache 2.0 for code. You keep your copyright; no assignment is required. Contributions to the specification also carry the patent commitments in the Community Specification License 1.0; any patent exclusion must be filed in [NOTICES.md](NOTICES.md) within 45 days of the contribution.

## Provenance

Every contribution records two things separately:

1. **The credited contributor:** a human, an AI, a human–AI collaboration, or an organization, credited by full name and role, pseudonym, or anonymously, as the contributor chooses.
2. **The submitting rights-certifier or facilitator:** the human or organization that makes the licensing declaration above.

For an AI contributor, give the AI's name and the system and version, and identify the facilitating human or organization.

## Pull requests

Pull requests are welcome. Open an issue first for any change to the requirements, so the change can be discussed and logged. In the pull request, reference the issue, name the requirement IDs affected, and state the contributor and facilitator as above.
