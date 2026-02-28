🌐 Language / 言語  
- 🇺🇸 [English](README.md)  
- 🇯🇵 日本語（current）

# Branching Reference Model (BRM)

![Linear vs BRM](/docs/img/linear_vs_brm_v2.png)

長期的なAI協働を安定化させるための構造フレームワーク。

---

## なぜAIとの協働は崩壊するのか（Why AI Collaboration Breaks）

AIとの対話が長くなるにつれ、表面上は安定しているように見えても、水面下では「構造的浸食」が進行しています：

- **意味の変質（Meaning Drift）**  
  基礎となる概念の定義が、時間の経過とともに微妙に変化していく。
- **錨（Anchor）の溶解**  
  直近の入力が優先され、初期に設定した重要な制約が「権威」を失っていく。
- **コンテキストの崩壊**  
  履歴が構造化されないまま蓄積され、未分化な「ノイズの場」と化す。
- **内部バイアスの蓄積**  
  曖昧な領域が、チェックされないまま「統計的にもっともらしい推論」で埋め尽くされる。

**これは知能の敗北ではない。構造的な連続性の問題である。**

---

## モデルの前提 — アンカーリング理論

BRMを定義する前に、まず理解すべき観測がある。

プロンプトは溶ける。

初期に与えた命令は、対話が蓄積するにつれて相対的な影響力を失う。  
AIの出力を支配するのは「最初の指示」ではなく、対話の中で再構築された参照場である。

この観測から導かれたのが、アンカーリング理論である。

- **[アンカーリング理論 — 溶ける入浴剤と、溶けない碇 (JP)](core/JP/Anchoring_Theory_Dissolving_Prompts_JP.md)**
- **[Anchoring Theory — Dissolving Prompts and the Permanent Anchor (EN)](core/EN/Anchoring_Theory_Dissolving_Prompts_EN.md)**

---

## 思考の原点（Thinking Phase）

*なぜこれを作ったのか？*

現在のLLMアーキテクチャにおいて、長期協働がなぜ崩壊するのか。その構造的解析を記した文書。

- **[AIとの長期協働における構造的ギャップ (JP)](core/JP/Structural_Gap_in_Long_Term_LLM_Collaboration_JP.md)**
- **[The Structural Gap in Long-Term LLM Collaboration (EN)](core/EN/Structural_Gap_in_Long_Term_LLM_Collaboration.md)**

---

## 構造比較（Structural Comparison）

| 比較項目 | ロール指定型プロンプト | コンテキスト蓄積型 | **BRM** |
| :--- | :--- | :--- | :--- |
| **長期安定性** | 低 | 中 | **高** |
| **ドリフト耐性** | 低 | 中 | **高** |
| **復旧性** | なし | 限定的 | **あり** |
| **構造の可視性** | 不透明 | 不透明 | **明示的** |

---

## Core Model（コア・モデル）

BRMの本質的な定義と論理構造。

- [Core Definition (JP)](core/JP/BRM_Core_Definition_JP.md)
- [Core Definition (EN)](core/EN/BRM_Core_Definition_EN.md)

---

## Compressed Theory Edition（要約理論版）

概念の本質を短時間で理解するためのエディション。

- [JP Theory](essay/JP/Illusion_of_Conversation_Compressed_Theory_JP.md)
- [EN Theory](essay/EN/Illusion_of_Conversation_Compressed_Theory_EN.md)

---

## Conceptual Essays（概念エッセイ）

AI協働の哲学に関する探求。

- [日本語エッセイ](essay/JP/)
- [English Essays](essay/EN/)

---

## Full Structured Model（完全構造化モデル）

完全な実装フレームワーク。

- [Full Model (JP)](full_model/JP/)
- [Full Model (EN)](full_model/EN/)

---

## Final Thought

AIの崩壊はカオスではない。

それは、設計のない重力が引き起こす必然である。

メモリを増やすことが解決策でないとするならば、  
我々は制御し損ねている「変数」に目を向けなければならない。

スコープ（参照範囲）は自然発生的な属性ではない。  
**それは、アーキテクチャ上の選択である。**
