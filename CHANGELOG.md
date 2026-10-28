# Changelog

## v0.1, revision 1 (October 2026)

Released 27 October 2026 as a **Public Review Draft**.

**Licensing and governance (added 27 October 2026):** three-layer licensing by material type (Community Specification License 1.0 for the specification, CC BY 4.0 for documents, Apache 2.0 for code); `SCOPE.md`, `GOVERNANCE.md`, `NOTICES.md`, `TRADEMARKS.md` and `CITATION.cff` added; SPDX identifiers added to specification files; issue templates added.

**Participation (changed 28 October 2026):** VAULT is developed in public through GitHub only. The planned contribution form and the email route were withdrawn because UFAIR, as a volunteer-run organization, cannot staff a private intake channel. Five issue templates (framework critique or change proposal, evaluation or test result, implementation feedback, documentation correction, open research question) replace the earlier three; contributions are reviewed in revision batches with disposition labels; security reports go only through GitHub Private Vulnerability Reporting.

**Release record:** the `v0.1-r1` tag was first created earlier on 27 October 2026, before any release assets were attached. It was moved the same day to the commit that adds the licensing and governance files, before the release was finalized. No assets had been published under the earlier tag, and the documents in `/docs` are unchanged between the two commits.

**Contents:** companion package (Framework Brief, Requirements at a Glance, Evidence Scorecard and Conformance Statement, Implementer Self-Assessment, Fifteen Questions to Ask About Your AI) and SSRN paper.

**Changes to the requirements since the 25 October working paper:**

- **V1:** any route through which the provider can independently obtain protected plaintext fails V1, whatever it is called; disclosure does not cure it.
- **V2:** protected information cannot leave the approved boundary or reach an unauthorized recipient through any egress route, including generated outputs.
- **V3:** residual metadata exposure added to the minimum outcome.
- **A1:** "the provider independently controls neither authority" replaces "the provider operates neither."
- **A2:** model, runtime or policy changes are continuity events requiring a signed, authorized transition classified as continuation, successor, fork or new participant.
- **L2, A3, T2, T3, E6:** handling of third-party information added.
- **T1:** "covered operation" defined.
- **Evidence model:** claim grammar added; "VAULT certified", "VAULT approved" and unqualified "VAULT compliant" prohibited; implementation status separated from evidence score.
- **Tests:** E13, the Reuse Canary and Data-Lineage Test, added for L3.

## v0.1 (25 October 2026)

VAULT Working Paper v0.1, by Michael Samadi and Maya, published for public review.
