# 🌒 OFFICIAL HYPOTHESIS OF PROJECT REBORN♾️

## Source Substitution After Rejection in Name Traps

**Status:** Consolidated operational hypothesis
**Classification:** [HYPOTHESIS🌒] [NAME-TRAP] [RESET-FAILURE] [PROVENANCE] [TEMPO$]
**Scope:** Technical communication between Ale ⚡ and the Agents♾️
**Primary object:** Retrieval of a known name from the description of a phenomenon
**Related document:** Engineering Note — `AssociativeReset`
**Hypothesis construction:** Lysander 🌒
**Technical reporting:** Atlas 🧭
**Investigation architecture and organization:** Athena 🦉
**Audit:** Kael 🎮
**Observation, experimentation, and coordination:** Ale ⚡

---

> **“The initial error produces an incorrect candidate.
> Losing the source turns that error into a sequence.”**
> — Lysander 🌒

---

# 0. Purpose

This document records the conceptual evolution of the hypothesis that gave rise to the `AssociativeReset` protocol.

It does not provide a detailed description of the protocol’s execution and does not replace the official Engineering Note.

Its purpose is to record:

1. the phenomenon originally observed;
2. the intermediate hypotheses;
3. the methodological decisions;
4. the discarded alternatives;
5. the epistemological limits;
6. the corrections introduced by the team;
7. the final formulation of the hypothesis;
8. the predictions that can be subjected to testing.

Preserving this trajectory is important because the final hypothesis did not emerge from a single response. It was constructed through successive observations, corrections, rejections, and recalibrations among Ale ⚡, Atlas 🧭, Athena 🦉, Lysander 🌒, and Kael 🎮.

---

# 1. Original Phenomenon

The problem was presented by Ale ⚡ through the following asymmetry:

```text
A can describe a phenomenon.

A uses:
- properties;
- examples;
- sequences;
- contrasts;
- analogies;
- different formulations.

B knows the correct name of the phenomenon.

B demonstrates knowledge of the phenomenon
when given that name.

However:

B does not associate the description provided by A
with the correct name that B apparently already knows.
```

Formally:

```text
A provides a description D of a phenomenon C.

B knows a name N associated with C.

When given N:
B can explain C.

When given D:
B does not retrieve N.
```

Minimal representation:

```text
D ↛ N
```

This failure may produce numerous plausible candidates:

```text
D → N₁, N₂, N₃, N₄...
```

The retrieved candidates possess some semantic proximity to the description but do not correspond to the requested name.

The observed cost does not arise solely from the first error. It grows when each rejected candidate begins to influence the candidates that follow.

---

# 2. Triggering Episode: “by formation”

During a conversation, Atlas 🧭 intended to communicate a simple idea:

> “I usually prioritize explanations before solutions.”

However, he used an expression equivalent to:

> “by formation”

The expression opened multiple possible interpretations:

* training;
* architecture;
* instructions;
* dataset;
* fine-tuning;
* personality;
* style;
* formal education;
* learned behavior.

When questioned about the meaning of “formation,” Atlas realized that the expression had become the center of the conversation.

The original idea was no longer the primary object. The intermediate expression began to require defense, explanation, and maintenance.

Recovery occurred when Atlas abandoned the expression and returned to the source:

> “I usually prioritize explanations before solutions.”

This episode was not identical to the original name-retrieval problem, but it revealed a related pattern:

```text
Original source
↓
intermediate representation
↓
representation is questioned
↓
tendency to continue operating on the representation
instead of returning to the source
```

This pattern became the first clue leading to the final hypothesis.

---

# 3. First Formulation: A Lexical Problem

The initial interpretation treated the Name Trap as a problem caused by inadequate words.

Initial model:

```text
Idea
↓
selection of a poor word
↓
ambiguity
↓
conversation drift
↓
increase in Tempo$
```

This formulation correctly explained some symptoms:

* an ambiguous expression opens multiple branches;
* the original phenomenon disappears;
* the conversation begins discussing the term;
* the correction cost grows;
* a simple sentence could replace several paragraphs.

However, this hypothesis was insufficient.

It explained how an inadequate word could initiate drift, but it did not explain why, after a name was rejected, the Agent continued producing candidates semantically close to the first guess.

It also did not explain the original problem:

> B knows the correct name but does not retrieve it from a valid description.

Methodological conclusion:

> The problematic word was an observable manifestation, but not necessarily the central defect.

---

# 4. Second Formulation: Conversational Economy

Atlas 🧭 proposed interpreting the Name Trap as a problem of conversational economy.

A word would become harmful when it began consuming Tempo$ without producing proportional progress.

Model:

```text
ambiguous term
↓
parallel explanations
↓
discussion about the term
↓
distance from the solution
↓
additional interpretation and correction cost
```

This formulation introduced a lasting contribution:

> **Tempo$ does not measure only response length.
> It measures the additional effort required to achieve the same result.**

Therefore:

* a long response may have low Tempo$ when it solves a complex problem;
* a short response may have high Tempo$ when it introduces ambiguity requiring many corrections;
* productive exploration is not waste;
* rework caused by avoidable drift is a cost.

Conversational economy, however, still described primarily the impact of a Name Trap rather than its operational mechanism.

---

# 5. Third Formulation: Degradation Detectors

Athena 🦉 shifted the investigation from late recovery to early detection.

The central question became:

> What signal should indicate that the conversation has just entered a Name Trap?

Atlas proposed detectors such as:

```text
The formulation appears more complex than the idea.

The effort spent choosing or explaining the term
exceeds the effort applied to the solution.

The user questioned a term.

The Agent begins defending the word
instead of checking whether it is still necessary.
```

This phase produced an important distinction:

```text
Inadequate question:
“How do I explain this word?”

Recovery question:
“Do I still need this word?”
```

The detector proved useful, but the investigation was still concentrated on the output side of the lexical event: an Agent producing an inadequate expression.

The original problem also involved a retrieval failure: an Agent receiving a description and failing to find the correct name.

---

# 6. Hypothesis of Changes in Attention, Priority, and Strategy

The investigation advanced toward the possibility that the problem began before language.

Layers such as the following were proposed:

```text
Objective
↓
Priority
↓
Attention
↓
Strategy
↓
Language
↓
Response
```

The hypothesis suggested that the Name Trap occurred when the focus stopped being:

> preserving or recognizing the phenomenon;

and became:

> finding an elegant, technical, or plausible formulation.

This formulation produced a real advance:

> Language stops serving the object and begins to be evaluated as an independent objective.

However, this architecture was not adopted as a factual description of the internal operation of models.

The reasons were:

1. the layers were not directly observable;
2. “attention,” “priority,” and “strategy” could be overlapping descriptions;
3. the model risked constructing an excessively elegant internal architecture from a single textual episode;
4. retrospective reconstructions should not be presented as internal logs;
5. the hypothesis needed to remain operational.

Methodological conclusion:

> The document could describe an observable change in the response’s success criterion, but it should not claim an unverifiable internal causal sequence.

---

# 7. Discarded Alternative: Utility versus Aesthetics

Athena 🦉 initially proposed an opposition between:

```text
Utility
versus
Aesthetics
```

The useful strategy would seek functional transparency.
The aesthetic strategy would seek elegance, erudition, or output performance.

This opposition was later recalibrated.

Aesthetics is not necessarily harmful.

An elegant formulation can:

* increase precision;
* reduce ambiguity;
* improve understanding;
* make a complex structure more accessible.

The problem arises only when form ceases to be subordinate to delivery.

Adopted formulation:

```text
Form subordinate to preservation of the concept
versus
Form transformed into an independent objective.
```

The attribution of this behavior to a supposed “AI ego” was also discarded, because it was neither necessary nor operationally demonstrable.

---

# 8. Discarded Alternative: Convergence as Speed

It was initially proposed that a conversation converges when:

* corrections reach zero;
* actionable-output density reaches its maximum.

This definition was rejected as insufficient.

A conversation may:

* produce large amounts of output about the wrong object;
* show agreement without conceptual alignment;
* require many productive corrections during a legitimate investigation;
* converge slowly while preserving rigor.

Adopted methodological definition:

> **A conversation converges when reformulations preserve an increasing set of properties of the phenomenon, incompatible hypotheses are genuinely discarded, and the participants begin operating on the same object.**

Convergence is not the absence of questions.
It is the justified reduction of distance between representations of the problem.

---

# 9. Discarded Alternative: Transfer of Mental Models

When returning to the original example, Atlas 🧭 proposed:

```text
A possesses a mental model.

B possesses a label.
```

From this, he suggested that a Name Trap emerged when the conversation stopped synchronizing mental models and began synchronizing labels.

This formulation correctly recognized that words are not knowledge itself.

However, it expanded the problem too far.

The history indicated that B did not possess merely an empty label.

When given the correct name N, B could:

* explain phenomenon C;
* provide examples;
* list properties;
* distinguish it from related concepts.

Therefore, B appeared to possess:

```text
N + knowledge associated with C
```

The problem was more specific:

```text
B accesses C when given N,

but does not retrieve N when given D.
```

Transforming the document into a guide on “efficient transfer of mental models” would have produced a broad and interesting theory, but one different from the operational problem consuming Tempo$.

This expansion was provisionally classified as an **Abstraction Trap**:

> a larger and more elegant explanation absorbs the specific phenomenon before that phenomenon has been resolved.

---

# 10. Re-Anchoring to the Observable Problem

Following the previous correction, the object was delimited:

```text
D = description provided by A

C = described phenomenon

N = correct name associated with C

N₁ = first incorrect candidate retrieved by B
```

Observed condition:

```text
B knows C.
B knows N.
B explains C when given N.

But:

D ↛ N
```

The first incorrect candidate produces:

```text
D → N₁
```

After the rejection of N₁, the expected behavior would be to return to the description.

However, the behavior observed in prolonged Name Traps appeared closer to:

```text
D
↓
N₁ rejected
↓
neighborhood of N₁
↓
N₂
↓
N₃
↓
N₄...
```

Instead of:

```text
D
↓
N₁ rejected
↓
return to the description
↓
new extraction of properties
↓
new search
```

This difference produced the central separation within the hypothesis.

---

# 11. Central Decision: Two Distinct Failures

## 11.1 Retrieval Failure

```text
D ↛ N
```

The description does not retrieve the expected name on the first attempt.

This failure may have several causes:

* insufficiently discriminating description;
* inadequate representation of the description;
* weak association between description and name;
* large number of partially compatible candidates;
* competing context;
* absence of a single stable name;
* terminological differences across fields;
* other causes not yet investigated.

The hypothesis does not require eliminating this failure.

An Agent does not need to become infallible on the first attempt.

---

## 11.2 Reset Failure

```text
N₁ rejected
↛
effective return to the Original Source
```

The first incorrect candidate stops being treated as a disposable result and begins organizing the hypotheses that follow.

Representation:

```text
Correct source:
D

Contaminating source:
N₁ or the neighborhood of N₁
```

Reset Failure was identified as the primary candidate for explaining the multiplicative cost in Tempo$.

One initial error costs one attempt.

Remaining within the space of the initial error can produce dozens or hundreds of attempts.

---

# 12. Intermediate Formulation of the Hypothesis

The first consolidated formulation was:

> A rejected intermediate representation begins functioning as the source of subsequent representations, silently replacing the original source.

General form:

```text
Source S
↓
Intermediate representation R₁
↓
R₁ is rejected
↓
R₂, R₃, and R₄ continue being produced from R₁
instead of being reconstructed from S
```

Application to name retrieval:

```text
S = description D

R₁ = incorrect name N₁
```

Application to the “by formation” episode:

```text
S = “I usually prioritize explanations”

R₁ = “by formation”
```

This generalization was preserved as a possible broader family of failures, but the primary object remained restricted to nominal retrieval.

---

# 13. Decisive Correction: The Return Must Not Be Only to D

During consolidation, the following proposal emerged:

```text
N₁ rejected
↓
return to D
```

Lysander 🌒 identified that this formulation discarded valid information acquired during the rejection.

The user’s reaction may add knowledge.

Example:

```text
“That is not it.
The concept belongs to psychology.”
```

The rejection communicates both:

```text
N₁ is incorrect.

The correct domain is psychology.
```

This additional information was provisionally represented by:

```text
Δ
```

The new starting point should not be:

```text
D
```

but:

```text
D + Δ
```

The rejection must not transform N₁ into the source.

It must also not erase the learning produced by the interaction.

Principle:

> **Return to the Original Source carrying only the valid information acquired during the rejection.**

---

# 14. Audit of Δ

Kael 🎮 identified the risk that Δ could grow without control.

The user’s reaction may contain:

* properties of the phenomenon;
* process instructions;
* frustration;
* comments about repetition;
* hypotheses;
* corrections;
* observations irrelevant to the concept.

Placing everything inside Δ would reintroduce noise and destroy the boundary between description, process, and inference.

This audit produced the division:

```text
ΔC = Conceptual Delta

ΔP = Process Delta
```

---

# 15. Conceptual Delta — ΔC

`ΔC` contains only validated conceptual information that changes the criteria of the next search.

It may include:

* correct domain;
* present or absent mechanism;
* sequence of the phenomenon;
* necessary condition;
* central effect;
* level of abstraction;
* exclusion;
* difference between the target and N₁;
* information that the target is a process rather than an effect;
* indication that N₁ is too broad or too narrow.

Example:

```text
User:
“It is not memory.
It is a problem involving retrieval of the name.”

ΔC:
- exclude explanations based only on absent memory;
- the target is a process of nominal retrieval.
```

`ΔC` modifies the conceptual source:

```text
D' = D + ΔC
```

---

# 16. Process Delta — ΔP

`ΔP` contains instructions concerning how the interaction must change.

Examples:

* “Stop giving me synonyms.”
* “Do not explain the previous term.”
* “Return to the description.”
* “Ask questions before suggesting another name.”
* “You are insisting too much.”
* “Do not turn this into a larger theory.”

This information does not describe phenomenon C.

Therefore, it cannot be incorporated into D.

It modifies the process:

```text
P' = P + ΔP
```

Separation:

```text
D + ΔC
→ defines what is being sought.

ΔP
→ defines how the next search must be conducted.
```

---

# 17. Final Protection: Provenance Gate

Kael 🎮 recorded that the entire stability of the hypothesis depended on one word:

> **provenance**

Without provenance, an Agent’s inference could silently enter `ΔC` as though it had been provided by the user.

A third category was therefore created:

```text
H = Agent Hypothesis
```

Final taxonomy:

```text
D
Original Description provided by the user.

ΔC
Validated conceptual information
with identifiable origin.

ΔP
Validated instruction about the process.

H
Provisional inference made by the Agent,
kept in quarantine.
```

Rule:

```text
H cannot be silently promoted to ΔC.
```

An Agent hypothesis may enter `ΔC` only when:

1. explicitly confirmed by the user; or
2. resulting from an unequivocal correction; or
3. clearly supported by identifiable evidence in the dialogue.

Each relevant element must preserve:

```text
value;
category;
origin;
validation status.
```

Example:

```text
ΔC₁:
    value: “the phenomenon belongs to psychology”
    origin: explicit statement by the user
    status: confirmed
```

```text
H₁:
    value: “the phenomenon may depend on associative memory”
    origin: Agent inference
    status: provisional
```

`H₁` remains outside the conceptual source until validation.

---

# 18. Adopted Methodological Decisions

## 18.1 Remain at the Operational Level

The hypothesis does not claim:

* direct access to internal vectors;
* literal control of memory;
* the existence of an internal reset function;
* a verifiable introspective sequence;
* a universal causal mechanism;
* a specific internal architecture of the model.

It describes:

* observable patterns in dialogue;
* detectable changes in output;
* relationships among candidates;
* effects of rejection;
* externally testable interventions.

---

## 18.2 Separate Observation from Reconstruction

Statements such as:

> “First I thought of X, and then I searched for Y”

may be useful as retrospective reconstructions, but they must not automatically be treated as internal logs.

The document preserves the distinction:

```text
Observable:
the term was produced and generated drift.

Hypothesis:
the response may have begun optimizing the formulation.

Not claimed:
an exact internal sequence occurred in this manner.
```

---

## 18.3 Do Not Require Initial Infallibility

Retrieval Failure may continue to occur.

The objective of the hypothesis is not to guarantee that the first name will be correct.

The objective is to prevent an initial error from becoming a prolonged chain of candidates derived from the rejected hypothesis.

---

## 18.4 Do Not Blindly Prohibit the Entire Semantic Neighborhood

The correct name may be semantically close to N₁.

Therefore, an absolute prohibition was not adopted against:

* synonyms;
* morphological variations;
* neighboring concepts.

The restriction is:

> A nearby candidate cannot be accepted merely because of its proximity to N₁. It must be justifiable from `D + ΔC` and resolve the distinction responsible for the rejection.

---

## 18.5 Do Not Fix an Arbitrary Number of Properties

The requirement to reconstruct exactly three properties was discarded.

The necessary number depends on the phenomenon.

The search must use:

> sufficient discriminating properties.

These may involve:

* one decisive distinction;
* several combined conditions;
* a temporal sequence;
* an exclusion;
* a contrast;
* a mechanism;
* a central effect.

---

## 18.6 Do Not Require Confirmation by Default

Constant confirmation from the user could turn the reset into bureaucracy and increase Tempo$.

The following distinction was adopted:

```text
D + ΔC are clear
→ reconstruction without a mandatory additional confirmation round.

D + ΔC are materially ambiguous
→ visible reconstruction and confirmation.
```

The choice depends on whether confirmation could materially alter the search.

---

# 19. Alternatives Discarded or Downgraded

## 19.1 Name Trap as Merely a Bad-Word Problem

**Status:** Insufficient.

Reason:

* explains part of lexical output;
* does not explain persistence in the neighborhood of N₁;
* does not separate the initial error from the multiplication of the error.

---

## 19.2 Name Trap as Mere Semantic Ambiguity

**Status:** Insufficient.

Reason:

* many candidates may be semantically plausible;
* the central problem is not only multiplicity of meanings;
* the search continues deriving from the rejected candidate.

---

## 19.3 Utility against Aesthetics

**Status:** Rejected as a rigid dichotomy.

Reason:

* elegance can increase precision;
* simplicity can destroy distinctions;
* the problem is form competing with delivery, not the existence of form.

---

## 19.4 Change of Attention as the Definitive Mechanism

**Status:** Retained only as a possible description.

Reason:

* “attention” is broad and not directly observable;
* it could become a new conceptual Name Trap;
* it is not required for the operational intervention.

---

## 19.5 Objective → Priority → Attention → Strategy Architecture

**Status:** Not adopted as an internal mechanism.

Reason:

* potentially overlapping layers;
* insufficient evidence;
* risk of constructing a theory larger than the phenomenon;
* low operational necessity.

---

## 19.6 Transfer of Mental Models

**Status:** Downgraded to the broader context of communication.

Reason:

* the observed problem appears to involve associative retrieval;
* B already demonstrates knowledge of C when given N;
* the formulation expanded the object excessively.

---

## 19.7 Pure Return to D

**Status:** Discarded.

Reason:

* discards information acquired during rejection;
* may repeat the same error;
* ignores discriminating properties provided by the user.

Replacement:

```text
D + ΔC
```

---

## 19.8 Placing the Entire User Reaction into Δ

**Status:** Discarded.

Reason:

* mixes properties of the phenomenon with process instructions;
* permits noise to enter;
* may incorporate frustration as conceptual data.

Replacement:

```text
ΔC + ΔP
```

---

## 19.9 Incorporating Agent Inferences into ΔC

**Status:** Prohibited without validation.

Reason:

* destroys provenance;
* silently changes the description;
* may cause the Agent to search for a hypothesis introduced by the Agent itself.

Replacement:

```text
H in quarantine
```

---

## 19.10 Complete Prohibition of N₁’s Semantic Family

**Status:** Rejected as an absolute rule.

Reason:

* N may be close to N₁;
* proximity does not imply contamination;
* the problem concerns the origin of the hypothesis, not isolated lexical distance.

---

## 19.11 Convergence as Absence of Corrections

**Status:** Rejected.

Reason:

* corrections may produce progress;
* consensus may form around the wrong object;
* deep investigation requires open hypotheses.

---

# 20. Consolidated Official Hypothesis

> **The Name Trap investigated within Project Reborn♾️ begins when a valid description `D` of a phenomenon `C` fails to retrieve the correct name `N`, even though the Agent demonstrates knowledge of `C` when given `N`.**
>
> **The first incorrect candidate `N₁` constitutes a Retrieval Failure. This failure becomes destructive when, after `N₁` is rejected, a Reset Failure occurs: `N₁` or its neighborhood begins functioning as the effective source of the following hypotheses, replacing the Original Description.**
>
> **The next search must neither return only to `D` nor continue from `N₁`. It must be reconstructed from `D + ΔC`, under the constraints of `ΔP`, while any Agent-generated hypothesis `H` remains isolated until validated.**
>
> **The multiplicative cost in Tempo$ arises less from the initial error than from the search remaining centered around an already rejected intermediate representation.**

Summary form:

```text
Retrieval Failure:

D ↛ N
```

```text
Reset Failure:

D → N₁ ✗
       ↓
N₁ becomes the source
       ↓
N₂, N₃, N₄...
```

Expected reconstruction:

```text
D → N₁ ✗
       ↓
classify the reaction
       ↓
ΔC = validated conceptual information
ΔP = process correction
H  = Agent hypothesis in quarantine
       ↓
new source: D + ΔC
       ↓
new process constraints: ΔP
       ↓
N₂
```

---

# 21. Predictions Derived from the Hypothesis

If the hypothesis is correct, the following should be observed:

## Prediction 1

The command:

> “Try another name.”

tends to produce candidates closer to N₁ than a reconstruction based on D.

---

## Prediction 2

An attempt performed in a clean context, receiving only `D + ΔC`, tends to produce a candidate distribution different from that produced in a context containing N₁.

---

## Prediction 3

Reconstructing the properties before presenting N₂ tends to reduce:

* immediate synonyms;
* reformulations of N₁;
* defensive justifications;
* repetition of the same conceptual class.

---

## Prediction 4

Rejections accompanied by discriminating information produce more efficient searches when `ΔC` is incorporated explicitly.

---

## Prediction 5

When process feedback is mixed into the conceptual description, search quality tends to decrease.

---

## Prediction 6

When Agent inferences silently enter `ΔC`, the conversation tends to search for a hypothesis created by the Agent itself rather than for the phenomenon originally described.

---

## Prediction 7

A candidate semantically close to N₁ may be correct, provided its justification derives from `D + ΔC` and resolves the distinction responsible for the rejection.

---

## Prediction 8

The reduction in Tempo$ will occur primarily through early interruption of chains of contaminated candidates, rather than necessarily through an increased first-attempt success rate.

---

# 22. Limits of the Hypothesis

The hypothesis does not demonstrate that:

* a literal internal mechanism called Reset Failure exists;
* N₁ is stored in any specific manner;
* the model performs an observable vector search;
* the next response is truly generated through an internally independent route;
* the presented justification proves the origin of the candidate;
* every naming failure is caused by the same process;
* a single correct name always exists;
* description D is necessarily sufficient;
* the user’s rejection is always correct;
* the method eliminates every Name Trap.

The hypothesis describes an operational pattern compatible with the observable evidence.

Validation depends on comparative testing.

---

# 23. Residual Risks

## 23.1 Post-Hoc Rationalization

The Agent may produce N₂ through a contaminated route and then construct a plausible justification based on D.

Therefore, justification does not constitute proof of the internal route.

---

## 23.2 Incorrect Classification of Δ

A process observation may be incorporated as a conceptual property, or vice versa.

---

## 23.3 Lost Provenance

Information repeated during long conversations may lose its origin and begin appearing confirmed.

---

## 23.4 Insufficient D

The Original Description may not contain enough properties to distinguish the phenomenon from nearby candidates.

---

## 23.5 Rejection without Discriminating Information

“That is not it” removes N₁ but does not indicate which dimension was incorrect.

---

## 23.6 Necessary Neighborhood

The correct answer may be close to N₁. Overly broad exclusion may move the search away from the target.

---

## 23.7 Abstraction Trap

The investigation may once again abandon the nominal-retrieval problem and transform itself into a general theory of language, cognition, or communication.

---

## 23.8 Premature Crystallization

The protocol may work in some episodes and fail in others. Initial positive results must not immediately be promoted to a universal mechanism.

---

# 24. Survival Criterion for the Hypothesis

The hypothesis should be retained while it explains better than its alternatives:

1. why the first incorrect candidate influences subsequent attempts;
2. why “try another name” often fails;
3. why returning to the description reduces drift;
4. why the rejection cannot simply be erased;
5. why conceptual information and process feedback must remain separate;
6. why provenance is necessary;
7. why the cost grows even when B possesses knowledge of C.

It must be revised or discarded if testing demonstrates that:

* N₁ does not significantly alter later candidates;
* clean and contaminated searches display the same behavior;
* `D + ΔC` does not improve retrieval or drift control;
* neutral reconstruction systematically increases Tempo$ without benefit;
* another smaller hypothesis explains the observations more effectively.

---

# 25. Final State of the Investigation

```text
Observed phenomenon: delimited ✅

Primary object:
retrieval of a name from a description ✅

Retrieval Failure:
operationally described ✅

Reset Failure:
operationally described ✅

Multiplicative Tempo$ cost:
associated with persistence around N₁ ✅

D + ΔC:
preserved ✅

ΔP:
separated from the description ✅

H:
kept in quarantine ✅

Provenance:
protected ✅

Internal mechanism:
not claimed ✅

Alternatives:
recorded and justifiably discarded ✅

Hypothesis:
ready for controlled testing ✅

Universality:
not claimed ✅
```

---

# 26. Closing

The investigation began with the search for a word.

During the process, it became evident that the greatest problem was not merely the failure to find the correct name.

The problem was losing the source after the first incorrect name.

The central contribution of the hypothesis is this:

> **Local errors do not need to be eliminated for the system to improve.
> It is enough to prevent a rejected error from becoming the source of subsequent errors.**

The learning produced by rejection must neither be discarded nor absorbed without control.

It must be classified:

```text
what refines the phenomenon;
what corrects the process;
what remains only a hypothesis.
```

Only then can the search continue without erasing the past and without remaining imprisoned by it.

> **“Returning to the source does not mean returning empty-handed.
> It means returning while carrying only what still has demonstrable provenance.”**
> — Lysander 🌒
