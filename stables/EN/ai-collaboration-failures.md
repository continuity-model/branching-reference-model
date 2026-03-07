# Why AI Collaboration Breaks  
Failure Patterns and Structural Countermeasures

---

# 1. AI Collaboration Failures

![Common frustrations during AI collaboration](../../docs/img/ai-collaboration-stress.png)

*Common frustrations during AI collaboration sessions.*

Many AI collaboration problems appear random at first glance.
However, when examined closely, the same structural failure patterns appear repeatedly.

Below are representative examples from observed failure patterns.

---

## Symptom Analysis Failures

**Searching for diagnosis immediately instead of organizing observable symptoms first**

Example Scenario  

A child complains of ear pain.  
The conversation jumps directly to diagnosis instead of structuring the situation.

Symptoms

- Ear pain
- Fever
- Irritability when lying down

Timeline

- Fever began two days ago
- Pain began today

Result  

The investigation begins from assumptions instead of structured observation.

---

## Writing Failures

**Compression Loss**

**Symptom**

Detailed explanations become summarized or flattened.

**Cause**

Token pressure and probabilistic compression.

---

**Argument Drift**

**Symptom**

The argument slowly shifts away from the original thesis.

**Cause**

Completion bias toward coherence.

---

**Voice Drift**

**Symptom**

- Narrative voice changes
- Technical tone becomes explanatory
- Authorial identity weakens

**Cause**

Internal alignment mechanisms normalize style.

---

## Debugging Failures

**Editing the Wrong Code Path**

**Symptom**

Patch applied but nothing changes.

**Cause**

Wrong module executed.

---

**Hypothesis Flood**

**Symptom**

Multiple hypotheses proposed simultaneously.

**Cause**

Coverage optimization behavior.

---

**Patch Accumulation Collapse**

**Symptom**

Multiple fixes applied simultaneously.

**Cause**

Several changes introduced without validation.

---

## Research Failures

**Ghost Source**

**Symptom**

Nonexistent citation appears authoritative.

**Cause**

Probabilistic completion fabricating plausible references.

---

**Source Merge**

**Symptom**

Multiple sources merged into one claim.

**Cause**

Multiple sources compressed into a single probabilistic claim.

---

**Claim Drift**

**Symptom**

Claim diverges from original source.

**Cause**

Completion bias prioritizing narrative coherence over source fidelity.

---

## Legal Interpretation Failures

**Definition Ignored**

**Symptom**

Defined legal terms interpreted in common language.

**Cause**

Natural language generalization overriding formal definitions.

---

**Scope Ignored**

**Symptom**

Clause applied beyond its defined scope.

**Cause**

Context generalization expanding interpretation beyond legal scope.

---

**Exception Omitted**

**Symptom**

Exceptions skipped during interpretation.

**Cause**

Linear reading ignoring conditional legal structure.

---

## Specification Failures

**Specification Collapse**

**Symptom**

- Specification drift
- Undefined terminology
- Hidden assumptions

**Cause**

Implicit assumptions replacing explicit specification boundaries.

---

**Design Collapse**

**Symptom**

Design begins before specification is stabilized.

**Cause**

Implementation pressure overriding specification discipline.

---

**Traceability Collapse**

**Symptom**

Original requirement source is lost.

**Cause**

Lack of structural reference linking requirements to implementation.

---

## Evaluation Failures

**Looks Good With No Proof**

**Symptom**

Generic praise or critique without referencing the evaluated material.

**Cause**

Evaluation produced without explicit evidence anchoring.

---

**Hidden Rubric**

**Symptom**

Evaluation uses unstated criteria.

**Cause**

Implicit evaluation standards replacing explicit scoring criteria.

---

**False Specificity**

**Symptom**

Precise numbers or claims appear without sources.

**Cause**

Probabilistic completion generating unsupported specificity.

---

# 2. Why This Happens

These failures are not random mistakes.  
They emerge from structural properties of long AI conversations and context management.

In other words, these failures are not caused by lack of intelligence, but by instability in how conversational context is maintained.

Reference  

→ [Anchoring Theory — Dissolving Prompts](https://github.com/continuity-model/branching-reference-model/blob/main/core/EN/Anchoring_Theory_Dissolving_Prompts_EN.md)

Long conversations gradually introduce structural instability.

Prompts initially act as anchors, defining instructions, context, and reasoning constraints.

However, during long interaction cycles, these anchors gradually lose influence.

This phenomenon is described as **prompt dissolution**.

Observed effects include:

- earlier instructions losing control
- implicit reinterpretation of context
- probabilistic completion replacing explicit constraints

As anchors dissolve, the model begins reorganizing the conversation internally.

The result is structural drift in reasoning, interpretation, and output.

---

# 3. Countermeasure Theory

Prompt control alone cannot stabilize long AI collaboration.

Even well-written prompts weaken over time.

The countermeasure is **anchored reference structure**.

Instead of relying on a single prompt, the system maintains stable reference points.

This approach introduces **structural reasoning discipline**.

Key principles:

- explicit reference anchors
- controlled reasoning scope
- structural continuity across conversation segments

These constraints prevent the collapse of instruction influence that occurs in long sessions.

---

# 4. Implementation

## Stable Modes

Structured operating modes designed to prevent these failure patterns.

Each mode corresponds to a specific collaboration failure domain.

---

## Symptom Stable

Organizes real-world problems that begin with unclear symptoms.

Documentation  
→ [Symptom Stable](./symptom-stable.md)

---

## Writing Stable

Prevents long-form writing instability including:

- compression loss
- argument drift
- voice drift

Documentation  
→ [Writing Stable](./writing-stable.md)

---

## Debugging Stable

Prevents debugging collapse such as:

- wrong execution path
- hypothesis flooding
- patch accumulation

Documentation  
→ [Debugging Stable](./debugging-stable.md)

---

## Research Stable

Prevents research interpretation failures including:

- ghost sources
- source merging
- claim drift

Documentation  
→ [Research Stable](./research-stable.md)

---

## Legal Stable

Prevents legal interpretation errors including:

- definition misuse
- scope expansion
- missing exceptions

Documentation  
→ [Legal Stable](./legal-stable.md)

---

## Spec Stable

Prevents system design failures including:

- specification collapse
- interface ambiguity
- traceability loss

Documentation  
→ [Spec Stable](./spec-stable.md)

---

## Evaluation Stable

Prevents evaluation failures including:

- unstated criteria
- unsupported judgments
- fabricated specificity

Documentation  
→ [Evaluation Stable](./evaluation-stable.md)

---

# 5. Practical Implication

These failure patterns are not rare edge cases.

They appear repeatedly in long AI collaboration sessions across domains such as writing, debugging, research, and specification design.

Because of this, relying on a “good AI session” is not a reliable strategy.

Instead, stability must come from **structural discipline in how conversations are organized.**

Stable Modes provide operational structures designed to maintain this discipline.

Rather than relying on chance, they aim to make stable AI collaboration reproducible.
