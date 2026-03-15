🌐 **Language / 言語**

- 🇺🇸 English (current)
- 🇯🇵 [日本語版はこちら](README_jp.md)

---

# Branching Reference Model (BRM)

![Linear vs BRM](docs/img/linear_vs_brm_v2.png)

A conceptual framework exploring structural stability in long-term AI collaboration.


Long conversations collapse because all tokens compete for attention.
BRM introduces a scoped reference structure.

![BRM Reference Structure](docs/img/brm_reference_structure.png)

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

If you'd like to experience one of these structures in practice, you can try a free Stable Mode:

→ **[Download Symptom Stable v1.2](https://github.com/continuity-model/branching-reference-model/releases/tag/symptom-stable-v1.2)**

---

# Concept Overview

The Branching Reference Model separates three layers of AI collaboration:

Conversation Structure  
↓  
Reasoning Process  
↓  
Inference Engine  

In this architecture:

User  
↓  
BRM (Conversation Structure)  
↓  
Stable Modes (Reasoning Protocols)  
↓  
LLM (Inference Engine)

BRM organizes the structure of discussion.  
Stable Modes guide reasoning behavior.  
The language model performs inference.

This separation allows reasoning strategies to evolve without destabilizing conversation structure.

---

# Repository Structure

This repository is organized as a progression from observed collaboration failures to a structural model.

Observed failures  
↓  
Prompt dissolution  
↓  
Reference instability  
↓  
Stable reasoning environments  
↓  
Branching Reference Model

The repository contains two main parts:

• Conceptual essays explaining the problem space  
• The core BRM model describing the proposed structure

---

# Essays

These essays explore structural issues observed in long AI conversations.

### AI Sees the Forest

Perspective differences between users and AI during reasoning.

→ **[Read essay](essay/EN/ai_sees_the_forest.md)**

---

### The Conversation Reference Problem

How reference drift appears in long AI conversations.

→ **[Read essay](essay/EN/ai_conversation_reference_problem.md)**

---

### Stable Environment and Perch

The idea of stabilizing reasoning through structured reference anchors.

→ **[Read essay](essay/EN/ai_stable_environment_and_perch.md)**

---

# Core Model

The formal conceptual description of the Branching Reference Model.

→ **[BRM Core Model v2](core/EN/BRM_Core_v2.md)**

This document defines the core primitives of BRM:

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

The package includes:

- the core mode file  
- activation instructions  
- an operating guide  
- quick reference  
- example failure cases  

allowing the mode to be used as a practical standalone tool.

Free release:

→ **[Download Symptom Stable v1.2](https://github.com/continuity-model/branching-reference-model/releases/tag/symptom-stable-v1.2)**

This mode can be used independently and also serves as a practical entry point to the structural reasoning ideas explored in BRM.

---

# How to Read This Repository

Readers can start anywhere, but the following order reflects the conceptual progression:

Essays  
↓  
Observed collaboration failures  
↓  
Reference instability  
↓  
Structural reasoning environments  
↓  
Branching Reference Model
