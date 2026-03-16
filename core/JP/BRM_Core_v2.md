# Branching Reference Model (BRM) Core v2

## 概要

Branching Reference Model (BRM) は、長期的なAI対話において発生する  
**参照の不安定性（reference instability）** を整理するための構造モデルである。

多くのAI対話は、単一の線形コンテキストの中で進行する。

会話が長くなるほど、

- 参照対象のずれ  
- トピックの衝突  
- 推論経路の混線  

が発生しやすくなる。

BRMはこれを解決するために  
**参照構造（reference structure）** を明示的に導入する。

---

## BRMの目的

BRMはAIの推論そのものを変更するものではない。

代わりに、以下を整理する。

- 会話構造  
- 参照関係  
- 推論スコープ  

つまりBRMは

```
Conversation Structure
↓
Reasoning Process
↓
Inference Engine
```

のうち

**Conversation Structure（対話構造）**を担当する。

---

## Design Principles

BRMは以下の設計原則に基づいている。

### 1. 推論を制御しない

BRMはAIの推論アルゴリズムを変更しない。  
推論そのものはLLMに任せる。

BRMはあくまで  
**推論が行われる参照環境**を整理する。

---

### 2. 構造を明示化する

通常のAI対話では、すべての履歴が  
単一の線形コンテキストとして扱われる。

BRMでは

- Node  
- Branch  
- Reference Scope  

という構造を導入し、  
思考経路を整理する。

---

### 3. 参照スコープを制御する

長い会話では、すべての履歴が  
同一の注意競合に参加する。

BRMでは  
**現在の思考対象を中心に参照スコープを整理する**。

これにより

- topic drift  
- context collision  
- reasoning interference  

を抑制する。

---

## 基本構造

![BRM Reference Structure](../docs/img/brm_reference_structure.png)

*Figure: BRM reference structure organizing conversation into scoped reasoning nodes.*

BRMは対話を以下の要素で整理する。

- Node  
- Branch  
- Reference Scope  

これらは長期対話における参照構造を安定させるための基本単位である。

---

# Node

Node（ノード）は  
**対話における独立した参照単位**である。

Node は単なるメッセージ単位ではない。  
また単なるトピック分類でもない。

BRMにおいて Node は、

**思考の局所的な区切り（local cognitive boundary）**

を表す。

例えば以下のようなものが Node になり得る。

- 問題の定義  
- 仮説  
- 設計議論  
- 検討中の案  
- 検証プロセス  

長い対話では、これらの思考単位が多数存在する。

通常のAI対話では、これらはすべて  
**単一の線形コンテキスト内で混在する。**

BRMではそれぞれを  
**独立した参照単位（Node）**として扱う。

---

# Branch

Branch（ブランチ）は  
**ノード間の思考接続**を表す。

会話は本来、単純な直線ではなく

- 分岐  
- 回帰  
- 並行検討  
- 参照関係  

を含む構造を持つ。

BRMではこの構造を  
**Branchとして明示化する。**

Branch は単なる親子関係を持つ **tree構造の枝**ではない。

むしろ、

**ノード間の意味的な思考接続（thought connection）**

を表す。

そのため、同じ Node 間でも  
複数の Branch が存在することがある。

---

# Reference Scope

Reference Scope（参照スコープ）は  
**AIが現在参照するコンテキスト範囲**を指す。

通常のAI対話では

```
全履歴
↓
注意機構
↓
推論
```

となるため、

すべてのトークンが  
**同一の注意競合に参加する。**

これにより

- unrelated context  
- topic drift  
- reasoning interference  

が発生する。

BRMでは  
参照スコープを **ノード構造に基づいて整理する**。

参照には解像度の差が存在する。

例：

Active Node  
→ 完全参照（full reference）

関連 Node  
→ 要約参照（summarized reference）

過去 Node  
→ ラベル参照（label reference）

この構造により  
長い対話でも **思考対象の焦点を維持できる。**

---

# Active Node

Active Node は  
**現在の議論対象となっているノード**である。

AIはこのノードを中心に  
参照スコープを構築する。

```
Active Node
↓
Related Nodes
↓
Reference Scope
```

この構造により、

長い会話でも  
**思考対象を安定して保持できる。**

---

# Structural Effect

BRMは以下の問題を緩和する。

### Reference Drift

長い会話の中で  
参照対象が徐々に変化してしまう問題。

---

### Topic Collision

複数のトピックが同一コンテキストで衝突する問題。

---

### Context Collapse

長い履歴の中で  
推論の焦点が不明瞭になる問題。

---

# BRMの位置付け

BRMはAIシステムの  
**推論アルゴリズムを変更するものではない。**

代わりに  
**対話構造を整理する層**として機能する。

```
User
↓
BRM（Conversation Structure）
↓
Stable Modes（Reasoning Protocol）
↓
LLM（Inference Engine）
```

この構造により

- 推論プロトコル  
- 会話構造  
- 推論エンジン  

を分離できる。

---

# Stable Modesとの関係

Stable Modes は  
**推論手順を安定させるためのプロトコル**である。

例：

- Symptom Stable  
- Review Stable  
- Writing Stable  

BRMはこれらのモードが動作するための  
**対話環境（conversation structure）**を提供する。

つまり

```
BRM = structure
Stable Mode = reasoning protocol
LLM = inference
```

という関係になる。

---

# まとめ

長期AI対話では、

- 参照の不安定化  
- 推論経路の混線  
- トピックの衝突  

が発生しやすい。

BRMは

**Node  
Branch  
Reference Scope**

という構造によって  
これらの問題を整理するための  
**対話構造モデル**である。

BRMは推論を制御するのではなく、

**対話の参照環境を安定化する。**
