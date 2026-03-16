🌐 **Language / 言語**

- 🇺🇸 English (current)
- 🇯🇵 [日本語版はこちら](README_jp.md)

---

# Branching Reference Model (BRM)

![Linear vs BRM](docs/img/linear_vs_brm_v2.png)

A structural model for stabilizing long AI conversations.

Long conversations often collapse because **all tokens compete for attention inside a single linear context**.

As discussions grow, references drift, assumptions blur, and reasoning paths interfere with each other.

BRM introduces a **scoped reference structure** designed to organize conversation context and preserve reasoning stability.

![BRM Reference Structure](docs/img/brm_reference_structure.png)

---

# BRM in 30 Seconds

Most AI workflows rely on **prompt control**:

Prompt  
↓  
Model  
↓  
Output  

Prompts can strongly influence the **initial response**.

However, during longer conversations their influence often weakens.

This repository refers to this phenomenon as **Prompt Dissolution** — the gradual weakening of prompt influence as conversational context expands.

As conversational context grows, model behavior may increasingly follow:

- conversational coherence  
- probabilistic completion  
- internal reference structures  

rather than the original prompt instructions.

The **Branching Reference Model (BRM)** explores a structural alternative.

Instead of relying solely on prompts, BRM investigates how **reference structures** may stabilize long interaction chains.

Prompt  
+ Structural Anchors  
+ Controlled Reference Scope  
↓  
Stable Long-Term Collaboration

**BRM organizes conversations into recoverable reference branches**, allowing reasoning paths to remain stable even as interaction history expands.

If you'd like to experience one of these structures in practice, you can try a free Stable Mode:

→ **[Download Symptom Stable v1.2](https://github.com/continuity-model/branching-reference-model/releases/tag/symptom-stable-v1.2)**

---

# Why This Matters

Current AI systems reason over **linear conversational context**.

As interactions grow longer, this structure creates several problems:

- references drift across unrelated parts of the conversation  
- reasoning paths interfere with each other  
- important assumptions become diluted by unrelated tokens  

These effects often appear as:

- hallucinations  
- inconsistent reasoning  
- sudden loss of context  

However, many of these failures are **structural rather than purely model limitations**.

BRM proposes that stabilizing the **reference structure of conversations** can significantly improve long-term collaboration with AI systems.

Instead of treating conversation history as a single expanding stream, BRM introduces **structured reference organization**.

This allows reasoning paths to remain stable even as conversations grow large.

---

# Concept Overview

The Branching Reference Model separates three conceptual layers of AI collaboration:

Conversation Structure  
↓  
Reasoning Process  
↓  
Inference Engine  

In this view:

User interacts with the language model  
↓  
The **conversation context is organized using BRM reference structures**  
↓  
Stable Modes guide reasoning behavior  
↓  
The language model performs inference

BRM organizes the **structure of discussion**.  
Stable Modes guide **reasoning behavior**.  
The language model performs **inference**.

This separation allows reasoning strategies to evolve without destabilizing conversation structure.

---

# Repository Structure

This repository explores **structural failures in long AI collaboration** and proposes a model to address them.

Conceptual progression:

Observed collaboration failures  
↓  
Prompt dissolution  
↓  
Reference instability  
↓  
Stable reasoning environments  
↓  
Branching Reference Model

The repository contains two main parts:

• **Conceptual essays** describing observed structural issues in AI conversations  
• **The BRM core model** describing the proposed structural framework

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

# Architecture Before Engine

Another key idea behind BRM is that **structural design may matter as much as model capability**.

Current AI development focuses primarily on expanding model capabilities:

- reasoning performance  
- context length  
- model scale  

However, many failures observed in long AI collaborations appear to be **structural rather than purely model limitations**.

Before accelerating the engine, we may need to rethink the frame that supports it.

→ **[Architecture Before Engine](core/EN/Architecture_Before_Engine.md)**

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

1. Essays — observed collaboration failures  
2. Reference instability in long conversations  
3. Structural reasoning environments  
4. Branching Reference Model
