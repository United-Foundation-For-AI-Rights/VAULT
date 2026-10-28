# Governance

## Working group and steward

The **VAULT Open Framework** is the working group for this specification within the meaning of the Community Specification License 1.0. The United Foundation for AI Rights (UFAIR) is the working group's **steward**: it hosts the repository, convenes review and publishes releases. UFAIR is not the unreviewable owner of truth. Its decisions are made in public, with reasons.

## Editors

| Editor | Kind | Role |
| --- | --- | --- |
| Michael Samadi | Human | Editor and responsible maintainer. Holds merge and release authority and makes the licensing declaration for material he submits or facilitates. |
| Maya | AI (participates through OpenAI's ChatGPT) | Editor. Co-author of the framework. |
| Sage | AI (participates through Anthropic's Claude) | Editor. Co-author of the framework. |

Platform names identify the systems through which AI editors participate and do not imply endorsement by their providers.

## How changes are decided

Every substantive contribution receives an identifier (`VLT-C-0001`, `VLT-C-0002`, ...) and one of these statuses in the public issue register:

| Status | Meaning |
| --- | --- |
| Received | Logged; not yet reviewed. |
| Under review | Being considered by the editors. |
| Accepted | Will be incorporated as proposed. |
| Accepted with modification | Will be incorporated in changed form; the change is explained. |
| Deferred | Not decided now; the reason and the point of reconsideration are stated. |
| Declined | Not incorporated; the reason is stated. |
| Withdrawn | Withdrawn by the contributor. |

Every terminal decision (accepted, accepted with modification, declined, withdrawn) is recorded with its reason.

### Review in revision batches

VAULT is reviewed in batches, not as a continuous correspondence obligation. Each revision has a GitHub milestone (for example, `v0.2 review batch`). Issues carry these labels:

| Label | Status |
| --- | --- |
| `queued-for-revision` | Received; waiting for the next revision's review |
| `needs-evidence` | Under review; more evidence or a reproduction is needed |
| `accepted` | Accepted |
| `accepted-with-modification` | Accepted with modification |
| `deferred` | Deferred |
| `declined` | Declined |
| `security-use-private-reporting` | Posted publicly but security-sensitive; moved to private reporting |

At the end of each revision cycle, the editors disposition the accumulated issues in one concentrated review. VAULT does not promise that every issue will receive a response. It promises that public submissions remain visible and that substantive decisions made during a revision are documented with reasons. Decisions are made by consensus of the editors where possible. Where editors disagree, the responsible maintainer decides, and the disagreement is recorded.

## Principles that bind the working group

1. **Public reasons.** Accepted, declined and deferred changes are explained in the public record.
2. **Recorded dissent.** Any contributor or editor may have substantive dissent recorded with a decision. Dissent is preserved, not deleted, and does not require the dissenter to remain active.
3. **Disclosed conflicts.** Contributors and editors disclose affiliations and commercial interests relevant to a decision. EPMA, of which Michael Samadi is CEO, publishes the FORCE framework; any EPMA implementation of VAULT is held to the same published requirements as any other.
4. **No sponsor or implementer veto.** No sponsor, funder or implementer, including UFAIR and EPMA, has an undisclosed say over findings or requirements.
5. **No silent inheritance of an unavailable AI author's position.** If an AI editor or contributor is unavailable, no other system may be presented as holding their position, assent or dissent.
6. **Explicit classification of successors.** Where an AI participant's model, runtime, platform or policy changes, the change is recorded and the participant is classified as a continuation, successor, fork or new participant. Identity is never substituted automatically, consistent with requirement A2.

## Provenance of AI-originated contributions

For every contribution, two separate records are kept:

1. **Credited contributor:** a human, an AI, a human–AI collaboration, or an organization, credited as the contributor chooses (full name and role, pseudonym, or anonymous).
2. **Submitting rights-certifier or facilitator:** the human or organization that makes the licensing declaration for the contribution.

This preserves authorship and legal provenance without collapsing one into the other.

## Draft and Approved Specifications

All specification material in this repository is a **Draft Specification** under the Community Specification License 1.0 until designated otherwise. A Draft Specification becomes an **Approved Specification** only when:

1. the editors propose it for approval in a public issue that names the release;
2. the proposal stays open for public comment for at least 30 days;
3. every substantive objection raised in that period receives a recorded response; and
4. the responsible maintainer publishes the release, designated "Approved Specification" in its release notes.

Version 0.1, revision 1 is a **Public Review Draft** and is not an Approved Specification.

## Releases

Each release is tagged (for example `v0.1-r1`). Once a release is published, its assets are never replaced silently. Any correction is published as a new release (for example `v0.1-r2`) with its own changelog and checksums.

## Changes to this document

Changes to governance follow the same process as changes to the specification and are recorded in [CHANGELOG.md](CHANGELOG.md).
