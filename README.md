🌐 **Language / 言語**

- 🇺🇸 English (current)
- 🇯🇵 [日本語版はこちら](README_jp.md)

---

# Branching Reference Model (BRM)

![Linear vs BRM](docs/img/linear_vs_brm_v2.png)

A conceptual framework exploring structural stability in long-term AI collaboration.

---

# BRM in 30 Seconds

Most AI workflows rely on prompt control:

Prompt  
↓  
Model  
↓  
Output

Prompts can strongly influence the initial response.

However, during long conversations their influence often weakens.  
This repository refers to this phenomenon as **Prompt Dissolution**.

As conversational context expands, model behavior may increasingly follow:

- conversational coherence  
- probabilistic completion  
- internal reference structures  

rather than the original prompt instructions.

The **Branching Reference Model (BRM)** explores a structural alternative.

Instead of relying solely on prompts, BRM investigates how reference structures may stabilize long interaction chains.

Prompt  
+ Structural Anchors  
+ Controlled Reference Scope  
↓  
Stable Long-Term Collaboration

BRM proposes organizing interaction into **recoverable reference branches**, allowing reasoning to remain stable even as conversation context expands.

This repository explores the structural ideas behind this approach.

If you'd like to experience one of these structures in practice, you can try a free Stable Mode:  
📦 **[Symptom Stable v1.2](https://github.com/continuity-model/branching-reference-model/releases/tag/symptom-stable-v1.2)**

---

# Repository Structure

This repository contains two main parts:

1. **Conceptual essays** explaining the problems observed in long AI conversations  
2. **The BRM core model** describing the proposed structural solution

## Essays (Conceptual Background)

These essays explore the observed structural issues in long AI interactions.

- [`essay/EN/ai_sees_the_forest.md`](essay/EN/ai_sees_the_forest.md)  
- [`essay/EN/ai_conversation_reference_problem.md`](essay/EN/ai_conversation_reference_problem.md)  
- [`essay/EN/ai_stable_environment_and_perch.md`](essay/EN/ai_stable_environment_and_perch.md)

The essays introduce several recurring patterns such as:

- perspective mismatch between users and AI
- instability of conversational references
- the need for stable reasoning environments

These observations gradually lead to the structural idea behind BRM.

## Core Model

The formal conceptual description of the model is provided here:

- [`core/EN/BRM_Core_v2.md`](core/EN/BRM_Core_v2.md)

This document defines the core primitives of the **Branching Reference Model**:

- Nodes  
- Branches  
- Reference Scope  

and explains how they organize long-term AI collaboration.

---

# Free Stable Mode (Symptom)

A lightweight practical tool derived from the structural ideas discussed in this repository.

**Symptom Stable Mode** stabilizes early-stage reasoning by enforcing structured observation before diagnosis or explanation.

Instead of jumping directly to conclusions, the mode organizes the situation through a simple triage structure:

- observation  
- timeline  
- severity  
- potential risk  
- clarification questions  

This approach helps prevent several common AI collaboration failures such as:

- premature conclusions  
- hypothesis flooding  
- reasoning drift  
- missed critical observations  

The package includes the core mode file, activation instructions, an operating guide, quick reference, and example failure cases, allowing the mode to be used as a practical standalone tool.

Free release:

- 📦 **[Download Symptom Stable v1.2](https://github.com/continuity-model/branching-reference-model/releases/tag/symptom-stable-v1.2)**

This mode can be used independently and also serves as a practical entry point to the structural reasoning ideas explored in BRM.

---

# How to Read This Repository

This repository is organized as a progression from observed collaboration failures to a proposed structural model.

Observed failures  
↓  
Prompt dissolution  
↓  
Prompt vs structural control  
↓  
Stable reasoning environments  
↓  
Structural gap in current systems  
↓  
Branching Reference Model

Readers can start anywhere, but the essays followed by the core model provide the clearest conceptual progression.
