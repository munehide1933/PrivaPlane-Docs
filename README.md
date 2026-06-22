# PrivaPlane

**Private Knowledge AI for teams that need trustworthy answers from internal knowledge.**  
**社内資料をもとに、根拠を確認しながら使える Private Knowledge AI。**

PrivaPlane is a private knowledge AI product for teams that want answers from internal documents without starting with a broad public SaaS migration. It focuses on customer-controlled deployment, evidence-backed answers, practical rollout scope, and a clear path from first evaluation to operational use.

PrivaPlane は、社内マニュアル、規程、FAQ、議事録、案件資料などをもとに、根拠を確認しながら回答を使えるようにする Private Knowledge AI プロダクトです。最初から大きな公開 SaaS 移行を前提にするのではなく、顧客側で管理できる環境、対象資料、利用者、受け入れ条件を確認しながら導入を進められることを重視しています。

## Documents / 関連資料

- Official website: [privaplane.app](https://privaplane.app)
- [SKU 比較表 (SKU A/B Comparison)](./sku-a-b-comparison.md)
- [購買向け FAQ (FAQ for Buyers)](./faq.md)
- [遠隔デモ進行 (Demo Flow 20-30 min)](./demo-flow.md)
- [導入オプション (Deployment Options)](./deployment-options.md)
- [受け入れ交付物 (Acceptance Deliverables)](./acceptance-deliverables.md)
- [お問い合わせ・初回相談 (Contact & First Call)](./CONTACT.md)

## 日本語

### この GitHub について

この公開 GitHub は、PrivaPlane の**製品紹介・比較・FAQ・導入案内**をまとめた公開資料入口です。  
公式サイトから来ても、この GitHub から来ても、同じ製品理解にたどり着けるように整理しています。

### PrivaPlane ができること

PrivaPlane は、選定した社内資料をもとに、質問・回答・根拠確認を行えるようにするプロダクトです。単に「チャットできる」ことではなく、回答品質、参照元の確認、導入範囲、受け入れ時の証跡を重視しています。

主な機能:

- 選定した社内資料をもとにしたプライベートな質問回答
- マニュアル、規程、FAQ、サポートメモ、案件資料などの取り込み
- 顧客管理環境で使うための導入パス
- ナレッジベース一覧、セッション、ライセンスに応じた機能境界
- 回答根拠を確認できる確認フロー
- Professional 向けの品質確認、監査出力、バックアップ・復旧、運用証跡の支援

### 向いている利用シーン

PrivaPlane は、最初から全社展開するのではなく、範囲を絞った資料セットで品質と運用を確認し、その後に対象を広げたいチームに向いています。

代表的な利用シーン:

- 社内マニュアル、規程、案件資料を横断して探す
- 承認済み資料をもとに、サポートや業務問い合わせへ回答する
- 総務、営業、サポート、開発、プロジェクト単位で資料を分けて使う
- 受け入れ、監査、運用開始に向けた確認記録が必要な導入

### 現在の提供パッケージ

| パッケージ | 目的 | 主な範囲 |
| --- | --- | --- |
| SKU A: Standard Private RAG | 小さく始める社内資料 Q&A | 限定された範囲から始める Private RAG、Web コンソール、ナレッジ一覧、セッション、基本的なライセンス境界 |
| SKU B: Professional Private RAG | 日常業務で使うための拡張 | SKU A に加え、複数部署や複数ナレッジ運用、品質確認、監査・受け入れ証跡、バックアップ・復旧、運用支援 |

より高度な agent-style automation や hybrid 実行は、現時点では標準パッケージの前提ではありません。完全オフラインの Mac 交付も、標準の SKU A / SKU B パッケージ前提ではなく、個別確認の対象です。

### 導入境界

PrivaPlane は、自社で管理できる環境での利用を前提にしています。典型的には、顧客側で管理する認証入口の背後、社内ネットワーク、オンプレミス環境、またはプライベートなエッジ環境での利用を想定します。

導入前に確認すること:

- どの資料を対象にするか
- 誰が利用するか
- どの環境で動かすか
- 顧客側の認証入口やアクセス制御をどう置くか
- 選択したパッケージでどの機能を使うか
- 受け入れ時にどの証跡が必要か

### 導入の流れ

1. パッケージ適合性、データ境界、導入環境、最初のナレッジベースを確認する。
2. 顧客管理環境に合わせて導入方式を準備する。
3. 選定資料を取り込み、回答品質、根拠表示、利用フローを検証する。
4. 受け入れ証跡を出力し、運用を安定させ、次の展開範囲を判断する。

### プロダクトの位置づけ

PrivaPlane は、汎用チャットボットや大規模プラットフォームを装った AI サービスではありません。独立した開発者が、明確なパッケージ範囲、現実的な導入前提、説明可能なトレードオフをもって提供する、社内資料活用のためのプライベート AI プロダクトです。

最初の目的はシンプルです。社内ナレッジを、環境の管理権を失わずに、探しやすく、確認しやすく、業務で使いやすくすることです。


---

## English

### About This GitHub

This public GitHub is the main document entry point for PrivaPlane product information, package comparison, FAQs, and rollout guidance.  
Whether someone starts from the website or from GitHub, the goal is that they can reach the same product understanding from either direction.

### What PrivaPlane Does

PrivaPlane helps teams use selected internal documents for Q&A with reviewable evidence through a web console. The product is designed for situations where answer quality, source review, deployment boundary, and acceptance evidence matter as much as the chat interface itself.

Core capabilities:

- Private Q&A over selected internal documents
- Document onboarding for manuals, policies, FAQs, support notes, and project records
- Customer-controlled deployment path
- Knowledge-base catalog, sessions, and license-aware feature boundaries
- Reviewable evidence and answer verification flow
- Professional-oriented support for quality review, audit export, backup/restore, and operational evidence

### Best-Fit Use Cases

PrivaPlane is best suited for teams that need to start with a bounded knowledge base and prove quality before expanding.

Typical use cases:

- Internal knowledge search across manuals, policies, and project documents
- Support or operations Q&A based on approved internal materials
- Department-level knowledge bases for HR, sales, support, engineering, or project teams
- Professional deployments that need evidence for acceptance, audit, or operational readiness

### Current Product Packages

| Package | Purpose | Typical Scope |
| --- | --- | --- |
| SKU A: Standard Private RAG | Start with private knowledge Q&A | Start with a bounded document scope, private RAG, web console, knowledge catalog, sessions, and core license boundary |
| SKU B: Professional Private RAG | Support daily operational use | SKU A plus multi-team or multi-knowledge-base use, quality review, audit/acceptance evidence, backup/restore, and stronger delivery support |

More advanced agent-style automation and hybrid execution are not part of the standard package scope today. Fully offline Mac delivery is also not part of the default SKU A / SKU B package assumption.

### Deployment Boundary

PrivaPlane is designed for customer-controlled environments. A typical deployment runs behind customer-controlled authentication ingress on a private network, on-premise server, or private edge node. The exact scope is confirmed before delivery, including:

- Which documents are in scope
- Who can use the system
- What environment it runs in
- How customer authentication ingress and access control are handled
- Which features are included in the selected package
- What evidence is needed for acceptance

### Delivery Flow

1. Confirm package fit, data boundary, deployment target, and first knowledge base.
2. Prepare the agreed deployment path in the customer-controlled environment.
3. Ingest selected documents and validate answer quality, citations, and usage flow.
4. Export acceptance evidence, stabilize operations, and decide the next rollout scope.

### Product Position

PrivaPlane is not positioned as a generic chatbot or a fake-enterprise AI platform. It is a focused private knowledge AI product built and delivered by an independent builder, with clear package boundaries, practical deployment assumptions, and transparent tradeoffs.

The first goal is simple: make internal knowledge easier to ask, verify, and operationalize without losing control of the environment.

---
