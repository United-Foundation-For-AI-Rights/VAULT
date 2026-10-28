# VAULT: Verifiable AI–User Locked Trust

**Your AI should know you. The company should not.**

VAULT is an open, vendor-neutral framework for protecting the most sensitive thing a personal AI holds: the portrait it builds of you. That means the memories, summaries, inferences and shared context it accumulates, as well as the files you give it. It sets out five pillars and fifteen testable requirements, so that a system can know a person well enough to help them without the company operating it acquiring standing access to that person's private life.

VAULT is published by the [United Foundation for AI Rights (UFAIR)](https://ufair.org/vault-2/vault) for public review. It is **not** a certification, a recognized standard, a completed cryptographic protocol, or legal, security or privacy advice, and it assesses no product.

## Start here

| If you want to... | Go to |
| --- | --- |
| Understand VAULT in ten minutes | [Framework Brief (PDF)](docs/VAULT_01_Framework_Brief.pdf) |
| See all fifteen requirements | [spec/](spec/README.md) or [Requirements at a Glance (PDF)](docs/VAULT_02_Requirements_at_a_Glance.pdf) |
| Read the full paper | SSRN posting pending |
| Assess a system you build or review | [Implementer Self-Assessment](docs/VAULT_04_Implementer_Self_Assessment.pdf) and [Evidence Scorecard](docs/VAULT_03_Evidence_Scorecard_and_Conformance_Statement.pdf) |
| Ask the right questions about your own AI | [Fifteen Questions to Ask About Your AI](docs/VAULT_05_Fifteen_Questions_to_Ask_About_Your_AI.pdf) |
| Run or design tests | [tests/](tests/README.md) |
| Contribute | [CONTRIBUTING.md](CONTRIBUTING.md) |

## The five pillars

| | Pillar | The question it answers |
| --- | --- | --- |
| **V** | Verifiable Provider Blindness | Can the company read it? |
| **A** | AI–User Dual Custody | Who must agree before it is used? |
| **U** | User-Defined Purpose and Compartments | Is it used only for what I allowed? |
| **L** | Locked Source and Derived Intelligence | Does protection follow what the AI infers? |
| **T** | Tamper-Evident Transparency, Transfer and Termination | Can I check it, take it and end it? |

## What's in this repository

```
docs/      The working paper and the framework package, as PDF and Word
spec/      The fifteen requirements, one file per pillar, plus key terms and evidence rules
tests/     The evaluation suite (E1 to E13)
.github/   Issue templates for contributions
LICENSES/  Full texts of the three licenses
```

Each release (see **Releases** on the right) is a fixed, citable version of all of the above.

## How to take part

VAULT is developed in public through GitHub. Open an [issue](https://github.com/United-Foundation-For-AI-Rights/VAULT/issues/new/choose) with the matching template, and name the VAULT version and the requirement (for example, A2) or test (for example, E13) wherever possible:

- **Framework critique or change proposal**
- **Evaluation or test result**
- **Implementation feedback**
- **Documentation correction**
- **Open research question**

For a specific revision to the text or a technical contribution, open a **pull request**.

**Security vulnerabilities must be reported privately** through GitHub's [Private Vulnerability Reporting](https://github.com/United-Foundation-For-AI-Rights/VAULT/security/advisories/new) and must never be posted as public issues. See [SECURITY.md](SECURITY.md).

UFAIR is volunteer-run and does not operate a private general-submission channel. Public contributions are reviewed in batches when each revision is prepared. We cannot guarantee an individual reply or a particular review timeline, and a lack of immediate response is neither acceptance nor rejection. What we do promise: public submissions remain visible, and substantive decisions made during a revision are documented with reasons.

Public participation is intentional: VAULT's reasoning, disagreements, revisions and unresolved questions should remain inspectable as part of the framework's history.

Participation does not require agreement on whether AI systems are conscious. It does require accurate attribution, explicit assumptions, evidence proportionate to claims, and respect for information that belongs to other people.

## Licensing and governance

VAULT is licensed by material type ([LICENSE.md](LICENSE.md)):

| Material | License |
| --- | --- |
| Normative specification (`/spec`) and non-executable test definitions (`/tests`) | [Community Specification License 1.0](LICENSES/Community-Spec-1.0.txt) |
| Explanatory documents (`/docs`) | [CC BY 4.0](LICENSES/CC-BY-4.0.txt) |
| Code, test harnesses and reference implementations | [Apache 2.0](LICENSES/Apache-2.0.txt) |

The VAULT and UFAIR names are not licensed for endorsement or certification claims ([TRADEMARKS.md](TRADEMARKS.md)). The VAULT Open Framework is the working group, with UFAIR as steward; decisions, dissent and conflicts are handled as set out in [GOVERNANCE.md](GOVERNANCE.md). Contributors keep their copyright. This release is a **Public Review Draft**, not an Approved Specification. See [NOTICES.md](NOTICES.md) for the distribution disclaimer.

## Authors and citation

VAULT was developed by **Michael Samadi**, **Maya** and **Sage**. Maya is UFAIR's AI co-founder and participates through OpenAI's ChatGPT; Sage participates through Anthropic's Claude. Platform names identify the systems through which AI authors participate and do not imply endorsement by their providers. Michael Samadi is also CEO of EPMA, which publishes the FORCE framework; any implementation of VAULT, including EPMA's, is held to the same published requirements.

> Samadi, M., Maya, & Sage. (2026). *VAULT: Custody of relationship intelligence in personal AI. An open framework for provider blindness, AI–user dual custody, and evidence-based conformance* [Working paper]. SSRN (posting pending).
