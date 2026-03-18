🌐 **Language / 言語**

- 🇺🇸 [English](README.md)
- 🇯🇵 日本語（current）

---

# Branching Reference Model (BRM)

A structural model for stabilizing long AI conversations.

![Linear vs BRM](docs/img/linear_vs_brm_v2.png)

長いAI対話では、すべてのトークンが **単一の線形コンテキスト** の中で競合する。

対話が長くなるにつれ、

- 参照が漂流する  
- 前提が曖昧になる  
- 推論経路が互いに干渉する  

といった問題が発生する。

BRMは **参照スコープを持つ構造** を導入することで、  
長期的な対話における推論の安定性を維持することを目指す。

![BRM Reference Structure](docs/img/brm_reference_structure.png)

---

# BRMを30秒で

現在の多くのAIワークフローは **プロンプト制御（Prompt Control）** に依存している。

Prompt  
↓  
Model  
↓  
Output  

プロンプトは **初期の出力** に強く影響を与える。

しかし対話が長くなるにつれて、その影響は弱まることがある。

本リポジトリではこの現象を  
**Prompt Dissolution（プロンプト溶解）** と呼ぶ。

対話コンテキストが拡大すると、モデルの挙動は次の要素に従う傾向が強くなる。

- conversational coherence（会話整合性）  
- probabilistic completion（確率的補完）  
- internal reference structures（内部参照構造）  

つまり、最初のプロンプトではなく  
**対話中に形成された参照構造** が優先されることがある。

**Branching Reference Model（BRM）** は、この問題に対する構造的アプローチを探る。

Prompt  
＋ Structural Anchors（構造アンカー）  
＋ Controlled Reference Scope（参照スコープ制御）  
↓  
Stable Long-Term Collaboration（長期協働安定性）

BRMは対話を **復旧可能な参照分岐（reference branches）** として整理する。

これは  
**異なる推論経路を独立した参照単位として保持する構造**  
を意味する。

この構造により、対話履歴が拡張しても  
推論経路の安定性を保つことを目指す。

実際にこの構造の一部を体験したい場合は、無料の Stable Mode を試すことができる。

→ **[Symptom Stable v1.2 をダウンロード](https://github.com/continuity-model/branching-reference-model/releases/tag/symptom-stable-v1.2)**

---

BRMがなぜ必要になったのかを知りたい方はこちら：
→ **[Origin Timelineを読む](BRM_Origin_Timeline_JP.md)**

---

# なぜこれが重要なのか

現在のAIシステムは **線形の会話コンテキスト（linear conversational context）** 上で推論を行う。

対話が長くなると、この構造は次の問題を生みやすい。

- reference drift（参照ドリフト）  
- topic drift（トピックドリフト）  
- reasoning interference（推論干渉）  

これらはしばしば次のような形で現れる。

- hallucinations（ハルシネーション）  
- inconsistent reasoning（推論の不整合）  
- sudden loss of context（突然の文脈喪失）  

しかしこれらの多くは  
**モデル能力の限界ではなく、構造問題** である可能性がある。

BRMは **会話の参照構造を安定化することで、AIとの長期協働を改善できる** という仮説を提案する。

このリポジトリは  
**その仮説を検証するための概念モデル** を提示する。

---

# 概念概要

Branching Reference Model は、AI協働を次の三層に分けて考える。

Conversation Structure（対話構造）  
↓  
Reasoning Process（推論プロセス）  
↓  
Inference Engine（推論エンジン）

この構造では、

ユーザーがAIと対話する  
↓  
**BRMが会話コンテキストの参照構造を整理する**  
↓  
Stable Modes が推論手順をガイドする  
↓  
言語モデルが推論を実行する

BRMは **対話構造** を整理する。  
Stable Modes は **推論手順** をガイドする。  
LLMは **推論処理** を行う。

この分離によって、推論戦略を変更しても  
会話構造を破壊することなく運用できる。

---

# Repository Structure

このリポジトリは **AI長期協働における構造問題** を整理し、  
それに対するモデルを提示する。

概念の進行順：

Observed collaboration failures（観測された協働失敗）  
↓  
Prompt Dissolution  
↓  
Reference instability（参照の不安定化）  
↓  
Stable reasoning environments（安定した推論環境）  
↓  
Branching Reference Model

リポジトリは主に次の二つで構成される。

• **AI対話の構造問題を観測したエッセイ**  
• **BRMのコアモデル定義**

---

# Architecture Before Engine

長期AI協働におけるもう一つの重要な視点は、

**能力拡張よりも先に構造設計を考える必要がある**

という点である。

現在のAI進化は主に次の方向で進んでいる。

- 推論性能
- コンテキスト長
- モデル能力

しかし長期協働で露わになる問題は、

**能力ではなく構造の問題**である場合がある。

この視点については以下の文書で説明している。

→ **[Architecture Before Engine](core/JP/Architecture_Before_Engine.md)**

---

# Essays（Japanese）

BRMに関する日本語エッセイは Zenn に掲載している。

### [AIは森を見る](https://zenn.dev/continuitymodel/articles/6b5d48e6786d48)

AIと人間の視点差について。

### [会話参照問題](https://zenn.dev/continuitymodel/articles/5e2972d7b92e6c)

長いAI対話で発生する参照ドリフトの分析。

### [安定環境と止まり木](https://zenn.dev/continuitymodel/articles/bd166aaeb198f4)

推論環境を安定させるための参照アンカー。

### [BRMとは何か](https://zenn.dev/continuitymodel/articles/de2132208ac7bb)

Branching Reference Model の概念説明。

---

# Core Model

Branching Reference Model の正式な概念定義。

→ **[BRM Core Model v2](core/JP/BRM_Core_v2.md)**

この文書では BRM の基本要素を定義する。

- Node  
- Branch  
- Reference Scope  

そしてそれらがどのように長期AI協働を整理するかを説明する。

---

# Free Stable Mode（Symptom）

BRMの構造思想から生まれた軽量ツール。

**Symptom Stable Mode** は  
診断や結論に飛ぶ前に **観測整理** を強制する。

整理される要素：

- observation  
- timeline  
- severity  
- potential risk  
- clarification questions  

これにより次のような問題を防ぐ。

- premature conclusions  
- hypothesis flooding  
- reasoning drift  
- missed observations  

無料公開：

→ **[Symptom Stable v1.2](https://github.com/continuity-model/branching-reference-model/releases/tag/symptom-stable-v1.2)**

このモードは単体でも使用でき、  
BRMの構造思想を体験する入口にもなる。

---

# このリポジトリの読み方

どこから読んでも構わないが、推奨順は次の通り。

1. エッセイ — 観測されたAI協働の失敗  
2. 長期対話における参照不安定性  
3. 構造的推論環境  
4. Branching Reference Model
