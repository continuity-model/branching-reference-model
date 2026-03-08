🌐 Language / 言語  
- 🇺🇸 [English](README.md)  
- 🇯🇵 日本語（current）

# Branching Reference Model (BRM)

![Linear vs BRM](/docs/img/linear_vs_brm_v2.png)

長期的なAI協働における構造的安定性を探るための概念フレームワーク。

---

## BRMを30秒で

現在の多くのAIワークフローは、プロンプトによってAIの挙動を制御しようとする。

Prompt  
↓  
Model  
↓  
Output

プロンプトは初期の出力に強く影響を与える。

しかし対話が長くなるにつれ、その影響は徐々に弱まることがある。  
本リポジトリではこの現象を **Prompt Dissolution（プロンプト溶解）** と呼ぶ。

コンテキストが拡大するにつれ、モデルの挙動は次の要素に従う傾向が強くなる。

- 会話の整合性  
- 確率的補完  
- 内部参照構造  

つまり、最初のプロンプトよりも **対話中に形成された参照構造** が優先されることがある。

**Branching Reference Model（BRM）** は、この問題に対する構造的アプローチを探る。

Prompt  
＋ 構造アンカー  
＋ 参照スコープ制御  
↓  
長期的な協働安定性

BRMは対話を **復旧可能な参照分岐（reference branches）** として整理することで、  
コンテキストが拡張しても推論の安定性を維持する可能性を探る。

本リポジトリは、その構造的アイデアを探究するものである。

---

## なぜAIとの協働は崩壊するのか

AIとの対話が長くなるにつれ、  
表面上は安定しているように見えても、水面下では構造的浸食が進行する。

- 意味の変質  
- 錨の溶解  
- コンテキストの崩壊  
- 内部バイアスの蓄積  

これは知能の敗北ではない。  
構造的な連続性の問題である。

より詳しい失敗パターンの整理：

- 🇯🇵 [なぜAIとの協働は崩れるのか](stables/JP/ai-collaboration-failures_JP.md)  
- 🇺🇸 [Why AI Collaboration Breaks](stables/EN/ai-collaboration-failures.md)

![AI Collaboration Stress](docs/img/ai-collaboration-stress.png)

---

## プロンプト溶解（Prompt Dissolution）

プロンプトはAIの初期挙動を強く制御する。

しかし対話が長くなると、その影響は徐々に弱まることがある。

![Prompt Roles Fade](docs/img/prompt_roles_fade.png)

初期の回答はプロンプトを強く反映するが、  
対話が進むにつれてモデルは次の要素に従いやすくなる。

- 会話の整合性  
- 確率的補完  
- 文脈再解釈  

この構造変化を **Prompt Dissolution** と呼ぶ。

---

## Prompt Control と Structural Control

プロンプト制御は **初期挙動** を形作る。

しかし長期対話では、追加の構造が必要になることがある。

![Prompt Control vs Structural Control](docs/img/prompt-control-vs-structural-control.png)

Prompt Control

- 単一の命令レイヤー

Structural Control

- 推論構造  
- 参照アンカー  
- 運用モード  
- ワークフロー制約  

詳しくは：

- 🇯🇵 [Prompt Control vs Structural Control](core/JP/prompt-control-vs-structural-control_JP.md)  
- 🇺🇸 [Prompt Control vs Structural Control](core/EN/prompt-vs-structural-control.md)

---

## 内部制御の進化

AI制御は段階的に進化してきた。

| 比較項目 | ロール指定 | コンテキスト蓄積 | アンカーリング | BRM |
| :--- | :--- | :--- | :--- | :--- |
| 長期安定性 | 低 | 中 | 高 | **非常に高い** |
| ドリフト耐性 | 低 | 中 | 高 | **構造的** |
| ルール保持持続性 | 低 | 中 | **高い** | **非常に高い** |
| ロール固定性 | 一時的 | 文脈依存 | **安定** | **構造的 + 復旧可能** |
| 復旧性 | なし | 限定的 | 部分的 | **あり** |
| 構造の可視性 | 不透明 | 不透明 | 半明示的 | **明示的** |

- ロール指定：振る舞いを宣言する  
- コンテキスト蓄積：履歴に依存して安定を試みる  
- アンカーリング：参照優先度と境界を設計する  
- BRM：参照スコープを明示的に構造化し、復旧可能にする  

---

## モデル以前の観測 — アンカーリング理論

プロンプトは溶ける。

AI出力を支配するのは、最初の命令ではなく、  
対話の中で再構築された参照場である。

- 🇯🇵 [アンカーリング理論 — 溶ける入浴剤と、溶けない碇](core/JP/Anchoring_Theory_Dissolving_Prompts_JP.md)  
- 🇺🇸 [Anchoring Theory — Dissolving Prompts and the Permanent Anchor](core/EN/Anchoring_Theory_Dissolving_Prompts_EN.md)

---

## 構造的ギャップ（Structural Gap）

長期協働が崩壊する根本原因の分析。

- 🇯🇵 [AIとの長期協働における構造的ギャップ](core/JP/Structural_Gap_in_Long_Term_LLM_Collaboration_JP.md)  
- 🇺🇸 [The Structural Gap in Long-Term LLM Collaboration](core/EN/Structural_Gap_in_Long_Term_LLM_Collaboration.md)

---

## コア定義（Core Model）

- 🇯🇵 [Core Definition](core/JP/BRM_Core_Definition_JP.md)  
- 🇺🇸 [Core Definition](core/EN/BRM_Core_Definition_EN.md)

---

## 外部拡張との違い

RAGや長大コンテキストは能力拡張である。  
BRMは参照制御である。

扱っている変数が異なる。

---

## エンジンの前にフレーム設計を

現在のAI進化は、主に能力拡張を軸としている。

- 推論性能  
- コンテキスト長  
- ベンチマーク  

しかし長期協働が露わにする制約は別にある。

それは **構造的連続性** である。

エンジンを加速させる前に、  
それを支えるフレームを再考する必要がある。

- 🇯🇵 [アーキテクチャはエンジンの前に — 長期LLM協働における最適化再定義](core/JP/Architecture_Before_Engine.md)  
- 🇺🇸 [Architecture Before Engine — Rethinking Optimization in Long-Term LLM Collaboration](core/EN/Architecture_Before_Engine.md)

---

## 最後に

AIの崩壊はカオスではない。

それは設計のない重力である。

メモリを増やすことが解決策でないならば、  
我々は参照構造を設計しなければならない。
