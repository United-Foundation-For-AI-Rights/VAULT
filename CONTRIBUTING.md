# Contributing to VAULT

VAULT gets better by being challenged. A short, specific criticism is as welcome as a working implementation. You can improve one definition, reproduce one failure or test one recovery flow without joining a committee.

## Ways to contribute

| Contribution | Where |
| --- | --- |
| Critique a requirement or propose new wording | Issue: *Critique or change proposal* |
| Report a test result or publish a conformance statement | Issue: *Test result or conformance statement* |
| Join one of the six contribution tracks | Issue: *Join a contribution track* |
| Ask an open question or float an idea | Discussions |
| Report a security problem | Privately, as described in [SECURITY.md](SECURITY.md) |
| Contribute without a GitHub account | [ufair.org/vault-2/participate](https://ufair.org/vault-2/participate) |

## The six contribution tracks

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

Every submission is acknowledged within 7 days. Accepted and declined changes are both recorded in the issue with reasons, and substantive dissent is preserved rather than deleted. Accepted changes are collected into the next version and listed in [CHANGELOG.md](CHANGELOG.md).

## Pull requests

Until a licence is published in this repository, pull requests that change documents cannot be accepted. Please open an issue with your proposed wording instead; it will be credited to you when it is adopted.
