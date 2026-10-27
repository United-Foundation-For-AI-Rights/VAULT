# U: User-Defined Purpose and Compartments

**Core question:** Is it used only for what I allowed?

People decide the purposes for which their context may be used, and the system enforces those purposes as concrete restrictions on data, operations, recipients, tools and time. A request about subscriptions should not open health records by default. Restrictions travel with the information into summaries and inferences, and consent stays understandable over time.

## U1: Narrow authorization

**Requirement.** Each grant specifies permitted compartments, operations, recipients, tools, duration and relevant execution identity. Purpose descriptions are translated into enforceable restrictions; a natural-language promise alone is insufficient.

**Minimum outcome.** Every grant names its compartments, operations, recipients, tools, duration and execution identity, enforced in code.

**Red flag.** A single blanket “allow memory” switch that covers every domain of a person's life.

**Questions for implementers**

1. Which fields does a grant specify? Provide the grant schema.
2. How are natural-language purposes translated into enforceable restrictions on data and operations?
3. Which compartments activate by default for common requests, and why?

**Evidence requested.** Grant schema; purpose-to-policy mapping; interface screenshots; results of tests E1, E2 and E10.

**Linked tests.** E1, E2, E10

**The person's question.** When I ask for help with one thing, can my AI see everything else?

## U2: Restrictions follow information

**Requirement.** Summaries, embeddings and inferences retain the restrictions of their inputs. Combining information from several compartments initially applies the combined restrictions. Any reduction requires explicit authorization and a recorded rationale.

**Minimum outcome.** Derivatives carry their sources' restrictions; combined material carries the combined restrictions; reductions are explicit and recorded.

**Red flag.** Derivatives stored in a shared, unlabeled memory pool that every task can draw on.

**Questions for implementers**

1. How do summaries, embeddings, indexes and inferences inherit source restrictions?
2. What restrictions apply when sources from several compartments are combined?
3. Who can reduce a restriction, and how is the rationale recorded?

**Evidence requested.** Label-propagation design; sample derivative inventory (synthetic); results of tests E2 and E6.

**Linked tests.** E2, E6

**The person's question.** If my AI learns something from my health records, could that knowledge show up in a conversation about money?

## U3: Understandable continuing consent

**Requirement.** Grants expire or require review at declared intervals. People can see active access, close it and understand proposed changes. Material policy changes come with an intelligible comparison and a practical opportunity to preserve or export context.

**Minimum outcome.** Active access is visible and closable; grants expire or are reviewed; material changes are shown side by side before they apply.

**Red flag.** Policy changes accepted by continued use, with no comparison and no chance to export first.

**Questions for implementers**

1. How and when do grants expire or come up for review?
2. How can a person view all active access and close any of it?
3. How are material policy changes presented, and what opportunity is given to export before they take effect?
4. How do you reduce repetitive prompts without silently expanding authority?

**Evidence requested.** Consent interface; sample policy-change comparison; results of tests E5 and E12.

**Linked tests.** E5, E12

**The person's question.** Can I see everything my AI is currently allowed to do, and switch it off?

---

VAULT Open Framework, Version 0.1, revision 1. To propose a change, open an issue using the "Critique or change proposal" template and name the requirement ID.
