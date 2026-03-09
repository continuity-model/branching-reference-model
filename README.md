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

This mode can be used independently and also serves as a practical entry point to the structural reasoning ideas explored in BRM.nd serves as a practical entry point to the structural concepts explored in BRM.

---

# How to Read This Repository

This repository is organized as a progression from observed collaboration failures to a proposed structural model.

Observed failures  
↓  
Prompt dissolution  
↓  
Prompt vs structural control  
↓  
Structured reasoning domains  
↓  
Structural gap in current systems  
↓  
Anchoring theory  
↓  
Branching Reference Model

Readers can start anywhere, but the sections above follow the conceptual progression used in this repository.

---

# What This Repository Proposes

This repository explores a structural perspective on AI collaboration.

Many current approaches attempt to control model behavior through methods such as:

- prompt engineering  
- larger context windows  
- improved reasoning capability  

These approaches primarily expand **model capability**.

This repository instead investigates **structural continuity in long interaction chains**.

The central idea explored here is that stable AI collaboration may benefit from:

- explicit reference anchors  
- structured reasoning domains  
- controlled reasoning scope  
- recoverable reference structures  

The Branching Reference Model (BRM) is presented as a conceptual framework that organizes these structural ideas.

Rather than proposing a specific implementation, the repository explores a **paradigm for structural governance of AI reasoning during extended collaboration**.

---

# Why AI Collaboration Breaks

Long conversations with AI systems often appear stable.

However, beneath the surface several patterns may emerge:

- meaning drift  
- dissolved reference anchors  
- contextual reinterpretation  
- accumulation of internal bias  

These effects are often interpreted as model inconsistency.

In many cases, they may instead reflect **structural continuity challenges in long interaction chains**.

Commonly observed patterns include:

- premature diagnosis instead of observation  
- argument drift in long writing sessions  
- hypothesis flooding during debugging  
- ghost sources during research  
- definition drift in legal reasoning  
- specification instability in design discussions  
- evaluation without explicit criteria  

Detailed breakdown:

- 🇺🇸 [Why AI Collaboration Breaks](stables/EN/ai-collaboration-failures.md)  
- 🇯🇵 [なぜAIとの協働は崩れるのか](stables/JP/ai-collaboration-failures_JP.md)

![AI Collaboration Stress](docs/img/ai-collaboration-stress.png)

---

# Prompt Dissolution

Prompts are commonly used to influence model behavior.

In many cases, prompts strongly shape the **initial generation context**.

During longer interactions, however, the influence of the initial prompt may weaken.

This effect is referred to here as **Prompt Dissolution**.

![How Prompt Roles Fade](docs/img/prompt_roles_fade.png)

Early responses may closely reflect prompt instructions, while later responses may increasingly follow conversational coherence and probabilistic completion patterns.

---

# Prompt Control vs Structural Control

Prompt engineering influences **initial model behavior**.

Long collaborative sessions may benefit from additional structural constraints.

![Prompt Control vs Structural Control](docs/img/prompt-control-vs-structural-control.png)

Prompt control:

- a single instruction layer influencing early generation

Structural control may introduce:

- explicit reasoning structures  
- reference anchors  
- operational modes  
- workflow constraints  

Further explanation:

- 🇺🇸 [Prompt Control vs Structural Control](core/EN/prompt-vs-structural-control.md)  
- 🇯🇵 [Prompt Control vs Structural Control](core/JP/prompt-control-vs-structural-control_JP.md)

---

# Structured Reasoning Domains

Different collaboration tasks involve different reasoning behaviors.

One way to organize these behaviors is through **task-specific reasoning domains**.

This repository refers to this conceptual organization as the **Stable Thinking Stack**.

- 🇺🇸 [Stable Thinking Stack](core/EN/stable-thinking-stack.md)  
- 🇯🇵 [Stable Thinking Stack](core/JP/stable-thinking-stack_JP.md)

Examples of reasoning domains include:

- observation  
- writing  
- debugging  
- research  
- legal interpretation  
- specification design  
- evaluation  

Each domain addresses a different class of reasoning instability.

---

# Structural Evolution of Internal Control

| Aspect | Role Prompting | Context Accumulation | Anchoring | BRM |
|------|------|------|------|------|
| Long-term stability | Low | Medium | High | Very High |
| Drift resistance | Low | Medium | High | Structural |
| Rule persistence | Low | Medium | High | Very High |
| Role fixation | Temporary | Context-dependent | Stable | Structural + Recoverable |
| Recoverability | No | Limited | Partial | Yes |
| Structural visibility | Hidden | Hidden | Semi-explicit | Explicit |

Conceptual interpretation:

- **Role Prompting** — behavioral instructions applied at initialization  
- **Context Accumulation** — stability emerging from conversational memory  
- **Anchoring** — prioritization of internal reference structures  
- **BRM** — explicit scoping architecture with recoverable reference slots  

---

# The Structural Gap

Current AI research often focuses on expanding capability.

Examples include:

- larger context windows  
- deeper reasoning chains  
- benchmark optimization  

However, long-term interaction sometimes exposes a different constraint:

**structural continuity of reference control.**

Discussion:

- 🇺🇸 [The Structural Gap in Long-Term LLM Collaboration](core/EN/Structural_Gap_in_Long_Term_LLM_Collaboration.md)  
- 🇯🇵 [The Structural Gap in Long-Term LLM Collaboration](core/JP/Structural_Gap_in_Long_Term_LLM_Collaboration_JP.md)

---

# Before the Model — Anchoring Theory

Prompts may dissolve over time.

During interaction, model behavior may instead become influenced by the strongest internal reference structures that emerge during conversation.

Anchoring theory explores this dynamic.

- 🇺🇸 [Anchoring Theory — Dissolving Prompts and the Permanent Anchor](core/EN/Anchoring_Theory_Dissolving_Prompts_EN.md)  
- 🇯🇵 [アンカーリング理論 — 溶ける入浴剤と溶けない碇](core/JP/Anchoring_Theory_Dissolving_Prompts_JP.md)

---

# Core Model

The Branching Reference Model (BRM) proposes a structural approach to maintaining reference continuity during extended collaboration.

Core definition:

- 🇺🇸 [Core Definition](core/EN/BRM_Core_Definition_EN.md)  
- 🇯🇵 [Core Definition](core/JP/BRM_Core_Definition_JP.md)

---

# Capability Expansion vs Structural Control

Approaches such as:

- RAG  
- extended context windows  
- reasoning optimization  

expand **capability**.

BRM explores a different dimension:

**reference scope stability during long interaction chains.**

These dimensions address different aspects of AI collaboration architecture.

---

# Architecture Before Engine

Many recent developments focus on increasing model capability.

Long interaction scenarios may highlight the importance of **structural continuity** alongside capability.

This perspective is explored in:

- 🇺🇸 [Architecture Before Engine — Rethinking Optimization in Long-Term LLM Collaboration](core/EN/Architecture_Before_Engine.md)  
- 🇯🇵 [アーキテクチャはエンジンの前に](core/JP/Architecture_Before_Engine.md)

---

# Full Structured Model

- 🇺🇸 [Full Model](full_model/EN/)  
- 🇯🇵 [Full Model](full_model/JP/)

---

# Final Thought

AI failure is not necessarily chaos.

In many cases it may reflect structural forces acting on long interaction chains.

Expanding context increases the size of the ocean.

Structural anchors may help determine how navigation occurs within it.
