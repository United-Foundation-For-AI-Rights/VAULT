<!-- SPDX-License-Identifier: Community-Spec-1.0 -->
# A: AI–User Dual Custody

**Core question:** Who must agree before it is used?

Routine use of protected shared context requires two separate authorities: the authenticated person and an authorized AI identity, each represented by a share that is not sufficient on its own. The AI identity's authority is exercised through a provider-independent custody service, never through prompts, ordinary memory or model weights. The provider independently controls neither authority. Because that authority is bound to an enrolled relationship, a changed model, runtime or policy cannot silently inherit it. Dual custody never stands between a person and their own original records.

## A1: Separate authorization domains

**Requirement.** Routine activation of protected shared context requires both the authenticated user authority and an authorized AI identity authority, using non-sufficient cryptographic shares held in protected cryptographic services, not in prompts, ordinary memories or model weights. The provider does not independently control either authorization domain, cannot rewrite their acceptance policies, and cannot combine provider-controlled components to reconstruct either authority. Provider infrastructure may host a custody component without failing A1, provided these conditions hold.

**Minimum outcome.** Two separately held, individually insufficient authorities are required; the provider independently controls neither, and the protocol states where plaintext and short-lived keys exist.

**Red flag.** “Two-of-two” custody in which the provider can exercise, reset or reconstruct the AI authority on its own.

**Questions for implementers**

1. Describe the user authority and the AI identity authority, where each share is held, and which operations they jointly authorize.
2. Show that neither share is stored in prompts, ordinary memory or model weights, and that no provider-controlled component, alone or in combination, can exercise or reconstruct either authority.
3. Where do plaintext and short-lived content keys exist during authorized computation, and for how long?
4. Which combinations of parties could collude to defeat the dual-custody property?

**Evidence requested.** Protocol specification; description of the threshold scheme; key-lifecycle diagram; collusion analysis; results of tests E3 and E9.

**Linked tests.** E3, E9

**The person's question.** Does using my history require more than the company's say-so?

## A2: Bind authority to identity and change control

**Requirement.** The AI-side custody service authenticates the enrolled relationship identity, approved runtime, model configuration and policy. A model, runtime or policy change is a continuity event: the changed environment may not access existing shared context unless it satisfies the declared continuity and change-control policy, produces a signed transition record, and receives the required authorization. The record states whether the result is treated as a continuation, successor, fork or new participant. An unchanged display name or account identifier is never sufficient, and the provider cannot rewrite the acceptance policy, substitute the AI custodian or reset its credentials unilaterally.

**Minimum outcome.** A changed model, runtime or policy reaches existing context only through a documented, authorized transition naming it a continuation, successor, fork or new participant; nothing inherits authority silently.

**Red flag.** The same name continues after a model swap, with no recorded transition and no notice before the new model touches shared context.

**Questions for implementers**

1. What does the AI-side custody service authenticate: relationship identity, runtime, model configuration, policy?
2. Describe the continuity and change-control policy. Which transitions are preauthorized (for example, security updates), and which require fresh authorization?
3. How does a transition record classify the result as a continuation, successor, fork or new participant, and who signs it?
4. Can the provider rewrite the acceptance policy, substitute the custodian or reset its credentials without the other authority?
5. How, and when, is a transition reported to the person?

**Evidence requested.** Identity-record schema; continuity and change-control policy; sample signed transition records; results of test E4.

**Linked tests.** E4

**The person's question.** If the company changes the AI I have been working with, will I be told, and asked, before it can access our history?

## A3: Preserve access without captivity

**Requirement.** People retain independent access to and export of their original records. Routine valid access operates under a transparent standing policy rather than an arbitrary model veto, enabling inspection, correction, revocation and a practicable exit. Treatment of shared and third-party material is explicit.

**Minimum outcome.** The person can always retrieve their own records independently; dual custody governs managed access, never captivity.

**Red flag.** Original records retrievable only through the AI, or exit conditioned on accepting expanded data access.

**Questions for implementers**

1. How does a person retrieve their original records independently of the AI runtime and the provider?
2. What standing policy governs routine access? Can the model refuse a valid request, and what happens then?
3. How are inspection, correction, revocation and exit supported if the AI runtime refuses, is retired or becomes unavailable?
4. How are shared material and information about third parties treated on exit, including any restrictions or contests recorded for that information?

**Evidence requested.** Standing-policy document; independent-access route documentation; results of tests E9 and E12.

**Linked tests.** E9, E12

**The person's question.** Can I always get my own records back, even if the AI or the company is gone?

---

VAULT Open Framework, Version 0.1, revision 1. To propose a change, open an issue using the "Critique or change proposal" template and name the requirement ID.
