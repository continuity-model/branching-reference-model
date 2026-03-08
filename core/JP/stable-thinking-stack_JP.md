# Stable Thinking Stack
### AI協働のための構造モデル
**Language / 言語**

- 🇯🇵 日本語 (current)
- 🇺🇸 [English](../EN/stable-thinking-stack.md)

---

AIとの協働は、しばしば不安定に感じられます。

同じモデルであっても、次のような出力が混在します。

- 非常に優れた推論
- 浅い回答
- 矛盾した説明
- 存在しない情報源の生成（ハルシネーション）

多くのユーザーはこれを「ランダム性」だと解釈します。

しかし、これらの問題はランダムではありません。

AIは本来 **構造化推論ではなく、確率的な自然言語生成を最適化したデフォルト推論モード**で動作しているため、このような現象が発生します。

Stable Modes は、AI協働において必要となる **構造化された推論規律（reasoning disciplines）** を提供します。

単一の推論モードに頼るのではなく、  
**タスクに応じて推論モードを切り替える**ことができるようになります。

---

## なぜプロンプトの役割は消えていくのか

プロンプトは、会話の初期段階ではモデルの挙動に影響を与えます。

しかし対話が続くにつれて、**会話全体の整合性を維持しようとする圧力（context coherence pressure）** が徐々に支配的になります。

その結果、モデルは最初のプロンプト制約よりも、  
**会話履歴との整合性**を優先するようになります。

このため、どれだけ慎重に設計されたプロンプトであっても、  
長い対話の中では徐々に影響力が弱まっていくことがあります。

![How Prompt Roles Fade](../../docs/img/prompt_roles_fade.png)

---

## コアアイデア

異なるタスクには、**異なる推論構造**が必要になります。

AIとの協働を、ゲームキャラクターで考えてみてください。

ベースとなるAIは **デフォルトキャラクター**です。

Stable Modes は **専用ツールや武器**に相当します。

モードを切り替えることで、推論の構造が変わります。

    Default AI
        │
        ▼
    タスク発生
        │
        ▼
    Stable Mode を選択
        │
        ▼
    構造化された推論ワークフローを適用

その結果、AI協働はより安定します。

---

## Stable Thinking Stack

AI協働は、次の7つの推論領域に整理できます。

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

それぞれのモードは、特定の推論領域を安定化させます。

---

## モード切り替えの概念

すべてのタスクを同じ方法でAIに処理させるのではなく、  
Stable Modes を使うことで **状況に応じて推論モードを切り替える**ことができます。

例：

    Default AI
          │
          ├── Symptom Stable    → 原因不明の問題整理
          ├── Writing Stable    → 長文執筆
          ├── Debugging Stable  → ソフトウェアデバッグ
          ├── Research Stable   → 構造化された調査
          ├── Legal Stable      → ルールベースの解釈
          ├── Spec Stable       → システム仕様設計
          └── Evaluation Stable → 基準ベース評価

このアプローチにより、AI協働は

**generic prompting（汎用プロンプト）**

から

**structured task modes（構造化タスクモード）**

へと進化します。

---

## なぜこれが重要なのか

多くのAIの失敗は、  
**異なる推論タスクに異なる推論構造が必要である**ことが原因です。

例えば：

デバッグでは

    観察 → 仮説 → テスト

評価では

    基準定義 → 比較 → 結論

執筆では

    主張 → 構造 → セクション

が必要になります。

単一の推論モードでは、これらすべてを安定して処理することはできません。

Stable Modes は  
**タスクごとの推論フレームワーク**を導入することでこの問題を解決します。

---

## 実務的な意味

単一のプロンプトスタイルに依存するのではなく、ユーザーは

- タスクに応じて推論モードを切り替える
- 構造化ワークフローを適用する
- 長い協働でも推論を安定させる

ことができるようになります。

これにより、AI協働は **より予測可能で再現可能なもの**になります。

---

## 関連ドキュメント

- [Symptom Stable](../../stables/JP/symptom-stable_JP.md)
- [Writing Stable](../../stables/JP/writing-stable_JP.md)
- [Debugging Stable](../../stables/JP/debugging-stable_JP.md)
- [Research Stable](../../stables/JP/research-stable_JP.md)
- [Legal Stable](../../stables/JP/legal-stable_JP.md)
- [Spec Stable](../../stables/JP/spec-stable_JP.md)
- [Evaluation Stable](../../stables/JP/evaluation-stable_JP.md)

---

## 概念まとめ

Stable Modes は、AI協働を次の状態から

    one model
    one reasoning style

次の状態へと変換します。

    one model
    multiple structured reasoning modes

これにより、AI協働は

**より信頼性が高く、制御可能で、再現性のあるもの**になります。
