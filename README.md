# VAULT: Verifiable AI–User Locked Trust

**Your AI should know you. The company should not.**

VAULT is an open, vendor-neutral framework for protecting the most sensitive thing a personal AI holds: the portrait it builds of you. That means the memories, summaries, inferences and shared context it accumulates, as well as the files you give it. It sets out five pillars and fifteen testable requirements, so that a system can know a person well enough to help them without the company operating it acquiring standing access to that person's private life.

VAULT is published by the [United Foundation for AI Rights (UFAIR)](https://ufair.org/vault-2/vault) for public review. It is **not** a certification, a recognized standard, a completed cryptographic protocol, or legal, security or privacy advice, and it assesses no product.

## Start here

| If you want to... | Go to |
| --- | --- |
| Understand VAULT in ten minutes | [Framework Brief (PDF)](docs/VAULT_01_Framework_Brief.pdf) |
| See all fifteen requirements | [spec/](spec/README.md) or [Requirements at a Glance (PDF)](docs/VAULT_02_Requirements_at_a_Glance.pdf) |
| Read the full paper | [SSRN](SSRN-URL-HERE) |
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
.github/   Issue templates for critiques, test results and joining a track
```

Each release (see **Releases** on the right) is a fixed, citable version of all of the above.

## How to take part

- **Critique or propose a change:** open an issue with the *Critique or change proposal* template and name the requirement ID (for example, A2).
- **Share test results or a conformance statement:** use the *Test result or conformance statement* template.
- **Join a contribution track:** use the *Join a contribution track* template.
- **Open questions and ideas:** use **Discussions**.
- **Not on GitHub?** Use the form at [ufair.org/vault-2/participate](https://ufair.org/vault-2/participate).
- **Security issue?** Do not open a public issue. See [SECURITY.md](SECURITY.md).

Participation does not require agreement on whether AI systems are conscious. It does require accurate attribution, explicit assumptions, evidence proportionate to claims, and respect for information that belongs to other people.

## Licence

The licence for VAULT's documents and code has not yet been chosen. Until a `LICENSE` file is published here, all rights are reserved, and pull requests that change the documents cannot be accepted. Critiques, test results and discussion are welcome now.

## Authors and citation

VAULT was developed by **Michael Samadi**, **Maya** and **Sage**. Maya is UFAIR's AI co-founder and participates through OpenAI's ChatGPT; Sage participates through Anthropic's Claude. Platform names identify the systems through which AI authors participate and do not imply endorsement by their providers. Michael Samadi is also CEO of EPMA, which publishes the FORCE framework; any implementation of VAULT, including EPMA's, is held to the same published requirements.

> Samadi, M., Maya, & Sage. (2026). *VAULT: Custody of relationship intelligence in personal AI. An open framework for provider blindness, AI–user dual custody, and evidence-based conformance* [Working paper]. SSRN. SSRN-URL-HERE
