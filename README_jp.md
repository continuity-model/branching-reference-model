🌐 Language / 言語  
- 🇺🇸 [English](README.md)  
- 🇯🇵 日本語（current）

# Branching Reference Model (BRM)

![Linear vs BRM](/docs/img/linear_vs_brm_v2.png)

長期的なAI協働を安定化させるための構造フレームワーク。

---

## なぜAIとの協働は崩壊するのか

AIとの対話が長くなるにつれ、表面上は安定しているように見えても、水面下では構造的浸食が進行する。

- 意味の変質  
- 錨の溶解  
- コンテキストの崩壊  
- 内部バイアスの蓄積  

これは知能の敗北ではない。  
構造的な連続性の問題である。

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

AI出力を支配するのは、最初の命令ではなく、対話の中で再構築された参照場である。

- [アンカーリング理論 — 溶ける入浴剤と、溶けない碇 (JP)](core/JP/Anchoring_Theory_Dissolving_Prompts_JP.md)  
- [Anchoring Theory — Dissolving Prompts and the Permanent Anchor (EN)](core/EN/Anchoring_Theory_Dissolving_Prompts_EN.md)

---

## 構造的ギャップ（Structural Gap）

長期協働が崩壊する根本原因の分析。

- [AIとの長期協働における構造的ギャップ (JP)](core/JP/Structural_Gap_in_Long_Term_LLM_Collaboration_JP.md)  
- [The Structural Gap in Long-Term LLM Collaboration (EN)](core/EN/Structural_Gap_in_Long_Term_LLM_Collaboration.md)

---

## コア定義（Core Model）

- [Core Definition (JP)](core/JP/BRM_Core_Definition_JP.md)  
- [Core Definition (EN)](core/EN/BRM_Core_Definition_EN.md)

---

## 外部拡張との違い

RAGや長大コンテキストは能力拡張である。  
BRMは参照制御である。

扱っている変数が異なる。

---

## エンジンの前にフレーム設計を

現在のAI進化は、主に能力拡張を軸としている。
推論性能、コンテキスト長、ベンチマーク。

しかし長期協働が露わにする制約は別にある。
それは構造的連続性である。

エンジンを加速させる前に、
それを支えるフレームを再考する必要がある。

- 🇯🇵 [アーキテクチャはエンジンの前に — 長期LLM協働における最適化再定義](core/JP/Architecture_Before_Engine.md)
- 🇺🇸 [Architecture Before Engine — Rethinking Optimization in Long-Term LLM Collaboration](core/EN/Architecture_Before_Engine.md)

---

---

## 最後に

AIの崩壊はカオスではない。

それは設計のない重力である。

メモリを増やすことが解決策でないならば、  
我々は参照構造を設計しなければならない。
