<!-- SPDX-License-Identifier: Community-Spec-1.0 -->
# L: Locked Source and Derived Intelligence

**Core question:** Does protection follow what the AI infers?

The protected asset is not only what a person supplies but what the system makes from it: memories, summaries, embeddings, indexes, inferred attributes and personalized adaptations. These derivatives are inventoried with their provenance, can be inspected and corrected, and do not quietly flow into training, analytics, advertising or unrelated human review.

## L1: An inventory with provenance

**Requirement.** Maintain a protected inventory of retained source objects and user-specific derivatives, including the dependencies needed to find affected memories, indexes, profiles, caches and adaptations. Record origin, purpose, model and policy version, time, compartment and retention rule. The inventory itself is protected.

**Minimum outcome.** Every retained source and derivative is inventoried with provenance, and the inventory is protected like the content.

**Red flag.** Caches, embeddings or personalized adaptations left out of the inventory.

**Questions for implementers**

1. Which retained sources and derivatives does the inventory cover: memories, summaries, indexes, profiles, caches, adapters?
2. What provenance is recorded for each item?
3. How is the inventory itself protected, given that it can reveal a person's life without the content?

**Evidence requested.** Inventory schema; synthetic sample inventory; results of tests E6 and E7.

**Linked tests.** E6, E7

**The person's question.** Is there a complete list of what my AI has kept about me?

## L2: Inspect and correct the portrait

**Requirement.** Provide a readable account of durable personal representations, supporting sources and whether each is stated, inferred or disputed. Confidence labels do not imply calibrated probabilities unless validated. A correction marks affected derivatives for review, recomputation, quarantine or removal. Information about third parties is minimized and labeled, and there is a defined process for restricting, contesting and deleting it, including a route for the third party where one is practicable.

**Minimum outcome.** People can read what is durably held about them, see what is stated, inferred or disputed, and correct it with effect on dependent derivatives; third-party information can be restricted, contested and deleted.

**Red flag.** A correction hides an item from view while it continues to shape responses.

**Questions for implementers**

1. What readable account of durable representations is provided? Does it distinguish stated, inferred and disputed items?
2. What happens to dependent derivatives when a person corrects or disputes an item?
3. Are confidence labels calibrated, and how is any lack of calibration communicated?
4. How is information about other people (family, colleagues, correspondents) labeled, minimized, restricted, contested and deleted?

**Evidence requested.** Portrait view; correction workflow; dependency handling; results of test E6.

**Linked tests.** E6

**The person's question.** Can I see what my AI believes about me, and fix what is wrong?

## L3: Govern every reuse

**Requirement.** Protected material must not silently enter shared training, external analytics, advertising systems or unrelated human review. Any authorized disclosure identifies its recipient, purpose and lifecycle consequences. Personalized adaptations remain in scope. Where influence cannot reliably be removed from a model, complete deletion is not promised.

**Minimum outcome.** No training, analytics, advertising or human review without specific authorization; adaptations are in scope; unremovable influence is disclosed in advance.

**Red flag.** “De-identified” or “aggregated” reuse exempted from authorization.

**Questions for implementers**

1. Can protected material, or anything derived from it, enter training, evaluation, analytics, advertising or human review? Under what authorization?
2. How are personalized adapters and other retained adaptations governed and deleted?
3. Where removal from a model is not reliable, how is that disclosed before the person agrees?

**Evidence requested.** Data-use policy; technical controls that exclude unauthorized destinations; pipeline lineage (ingestion manifests, data catalogs, access records, authorization receipts); adapter lifecycle documentation; results of proposed test E13.

**Linked tests.** E13 (proposed)

**The person's question.** Could what I share be used to train or improve other products?

---

VAULT Open Framework, Version 0.1, revision 1. To propose a change, open an issue using the "Critique or change proposal" template and name the requirement ID.
