# The Stable Thinking Stack
### A Structural Model for AI Collaboration
**Language / 言語**

- 🇺🇸 English (current)
- 🇯🇵 [日本語](../JP/stable-thinking-stack.md)
---

AI collaboration often feels inconsistent.

The same model can produce:

- excellent reasoning
- shallow answers
- contradictions
- hallucinated references

Many users interpret this as randomness.

However, these failures are not random.

They emerge because AI operates in a **default reasoning mode optimized for fluent probabilistic language generation rather than structured reasoning**.

Stable Modes introduce **structured reasoning disciplines** designed for different collaboration tasks.

Instead of relying on one generic reasoning mode, the user can **switch operational modes depending on the task**.

---

## Why Prompt Roles Often Fade

Prompt instructions can influence the model at the start of a conversation.

However, as dialogue continues, **context coherence pressure gradually dominates the reasoning process**.

The model prioritizes maintaining internal consistency with the conversation history rather than preserving the original prompt constraints.

This is why carefully written prompts often appear to “fade” during long interactions.

![How Prompt Roles Fade](../docs/img/prompt_roles_fade.png)

---

## The Core Idea

Think of AI collaboration like a game character.

The base AI is the **default character**.

Stable Modes are **specialized tools or weapons**.

Each mode changes how reasoning is structured.

    Default AI
        │
        ▼
    Task appears
        │
        ▼
    Select Stable Mode
        │
        ▼
    Apply structured reasoning workflow

The result is more stable collaboration.

---

## The Stable Thinking Stack

AI collaboration can be organized into seven reasoning disciplines.

    Observation
        │
    Symptom Stable

    Expression
        │
    Writing Stable

    Debugging
        │
    Debugging Stable

    Investigation
        │
    Research Stable

    Interpretation
        │
    Legal Stable

    System Design
        │
    Spec Stable

    Judgment
        │
    Evaluation Stable

Each mode stabilizes a specific category of reasoning.

---

## Mode Switching Concept

Instead of asking AI to perform every task in the same way, Stable Modes allow **mode switching depending on the situation**.

Example:

    Default AI
          │
          ├── Symptom Stable    → diagnosing unclear problems
          ├── Writing Stable    → long-form writing
          ├── Debugging Stable  → software debugging
          ├── Research Stable   → structured investigation
          ├── Legal Stable      → rule-based interpretation
          ├── Spec Stable       → system specification
          └── Evaluation Stable → criteria-based judgment

This approach turns AI collaboration from **generic prompting** into **structured task modes**.

---

## Why This Matters

Most AI failures occur because different reasoning tasks require **different reasoning structures**.

For example:

Debugging requires:

    observe → hypothesize → test

Evaluation requires:

    define criteria → compare → conclude

Writing requires:

    thesis → structure → sections

A single reasoning mode cannot reliably support all of these tasks.

Stable Modes solve this by introducing **task-specific reasoning frameworks**.

---

## Practical Implication

Instead of relying on a single prompt style, users can:

- switch reasoning modes depending on the task
- apply structured workflows
- maintain stable reasoning during long collaboration

This makes AI collaboration more **predictable and reproducible**.

---

## Related Documents

- [Symptom Stable](../stables/EN/symptom-stable.md)
- [Writing Stable](../stables/EN/writing-stable.md)
- [Debugging Stable](../stables/EN/debugging-stable.md)
- [Research Stable](../stables/EN/research-stable.md)
- [Legal Stable](../stables/EN/legal-stable.md)
- [Spec Stable](../stables/EN/spec-stable.md)
- [Evaluation Stable](../stables/EN/evaluation-stable.md)

---

## Concept Summary

Stable Modes transform AI collaboration from:

    one model
    one reasoning style

into:

    one model
    multiple structured reasoning modes

This enables **more reliable, controllable, and reproducible AI collaboration.**
