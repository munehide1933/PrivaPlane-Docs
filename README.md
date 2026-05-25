# PrivaPlane

**Private Knowledge AI for teams that need answers from internal knowledge.**  
**社内資料をもとに、根拠を確認しながら回答する業務AI。**

PrivaPlane is a founder-led private knowledge AI product for organizations that want to use internal documents for question answering without turning the first step into a broad public SaaS migration. It focuses on private RAG, document onboarding, local model execution, licensing boundaries, and delivery evidence that can be reviewed before production rollout.

PrivaPlane は、社内マニュアル、規程、FAQ、議事録、案件資料などをもとに、必要な情報を探して回答を支援する社内向け AI プロダクトです。公開 SaaS へ一気に移行するのではなく、自社で管理できる環境・資料範囲・利用者・権限を確認しながら、小さく導入して検証できることを重視しています。

## Documents / 関連資料

- [SKU 比較表 (SKU A/B Comparison)](./sku-a-b-comparison.md)
- [購買向け FAQ (FAQ for Buyers)](./faq.md)
- [遠隔デモ進行 (Demo Flow 20-30 min)](./demo-flow.md)
- [導入オプション (Deployment Options)](./deployment-options.md)
- [受け入れ交付物 (Acceptance Deliverables)](./acceptance-deliverables.md)
- [お問い合わせ・初回相談 (Contact & First Call)](./CONTACT.md)

## 日本語

### PrivaPlane ができること

PrivaPlane は、選定した社内資料からプライベートなナレッジベースを作り、Web コンソール上で質問・回答に利用できるようにするプロダクトです。単に「チャットできる」ことではなく、回答品質、参照元の確認、導入範囲、受け入れ時の証跡を重視しています。

主な機能:

- 選定した社内資料をもとにしたプライベートな質問回答
- マニュアル、規程、FAQ、サポートメモ、案件資料などの取り込み
- 自社管理環境で利用するためのローカルモデル実行パス
- ナレッジベース一覧、セッション、ライセンスに応じた機能境界
- 回答根拠を確認できる検索・参照情報
- Professional 向けの監査出力、バックアップ・復旧確認、導入証跡の支援

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
| SKU A: Standard Private RAG | 小さく始める社内資料 Q&A | 選定資料、プライベート Web コンソール、RAG Q&A、ナレッジ一覧、セッション、ライセンス境界 |
| SKU B: Professional Private RAG | 日常業務で使うための拡張 | SKU A に加え、複数ナレッジベースまたはプロジェクト、品質確認、監査・受け入れ証跡出力、バックアップ・復旧、運用支援 |

より高度なエージェント型自動化や、完全オフラインの Mac 利用については個別相談の対象ですが、標準パッケージの前提ではありません。

### 導入境界

PrivaPlane は、自社で管理できる環境での利用を前提にしています。典型的には、顧客側で管理する認証入口の背後、社内ネットワーク、オンプレミス環境、またはプライベートなエッジ環境での利用を想定します。

導入前に確認すること:

- どの資料を対象にするか
- 誰が利用するか
- どの環境で動かすか
- 選択したパッケージでどの機能を使うか
- 受け入れ時にどの証跡が必要か

### 導入の流れ

1. パッケージ適合性、データ境界、導入環境、最初のナレッジベースを確認する。
2. 顧客管理環境に合わせてリリーススタックとローカルモデル実行環境を準備する。
3. 選定資料を取り込み、回答品質、根拠表示、利用フローを検証する。
4. 受け入れ証跡を出力し、運用を安定させ、次の展開範囲を判断する。

### プロダクトの位置づけ

PrivaPlane は、汎用チャットボットや大規模プラットフォームを装った AI サービスではありません。独立した開発者が、明確なパッケージ範囲、現実的な導入前提、説明可能なトレードオフをもって提供する、社内資料活用のためのプライベート AI プロダクトです。

最初の目的はシンプルです。社内ナレッジを、環境の管理権を失わずに、探しやすく、確認しやすく、業務で使いやすくすることです。


---

## English

### What PrivaPlane Does

PrivaPlane helps teams create a private knowledge base from selected internal documents and use it through a web console for RAG-based Q&A. The product is designed for situations where answer quality, source review, deployment boundary, and acceptance evidence matter as much as the chat interface itself.

Core capabilities:

- Private knowledge-base Q&A over selected internal documents
- Document onboarding for manuals, policies, FAQs, support notes, and project records
- Local model execution path for customer-controlled environments
- Knowledge-base catalog, sessions, and license-aware feature boundaries
- Reviewable retrieval evidence and acceptance-oriented delivery support
- Optional Professional delivery support for audit export, backup/restore checks, and operational evidence

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
| SKU A: Standard Private RAG | Start with private knowledge Q&A | Selected documents, private web console, RAG Q&A, knowledge catalog, sessions, and license boundary |
| SKU B: Professional Private RAG | Support daily operational use | SKU A plus multiple knowledge bases or projects, quality dashboard, audit/acceptance export, backup/restore, observability, and stronger delivery support |

More advanced agent-style automation or fully offline Mac usage can be discussed case by case, but they are not the default package scope.

### Deployment Boundary

PrivaPlane is designed for customer-controlled environments. A typical deployment can run behind customer-controlled authentication ingress on a private network, on-premise server, or private edge node. The exact scope is confirmed before delivery, including:

- Which documents are in scope
- Who can use the system
- What environment it runs in
- Which features are included in the selected package
- What evidence is needed for acceptance

### Delivery Flow

1. Confirm package fit, data boundary, deployment target, and first knowledge base.
2. Prepare the release stack and local model runtime in the customer-controlled environment.
3. Ingest selected documents and validate answer quality, citations, and usage flow.
4. Export acceptance evidence, stabilize operations, and decide the next rollout scope.

### Product Position

PrivaPlane is not positioned as a generic chatbot or a fake-enterprise AI platform. It is a focused private knowledge AI product built and delivered by an independent builder, with clear package boundaries, practical deployment assumptions, and transparent tradeoffs.

The first goal is simple: make internal knowledge easier to ask, verify, and operationalize without losing control of the environment.

---
