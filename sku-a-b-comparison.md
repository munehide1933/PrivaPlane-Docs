# SKU A/B Comparison

**PrivaPlane currently focuses on two paid delivery packages: SKU A and SKU B.**  
**PrivaPlane は、現在 SKU A と SKU B の 2 つの有償導入パッケージを中心に提供します。**

This document is written for buyers and project owners who need to quickly understand the difference between the two packages before a scoping call.

この資料は、商談前に SKU A / SKU B の違いをすばやく確認したい購買担当者・導入担当者向けの比較表です。

---

## 日本語

### 比較表

| 観点 | SKU A: Standard Private RAG | SKU B: Professional Private RAG |
| --- | --- | --- |
| 目的 | 小さく始める社内資料 Q&A | 日常業務で使うための複数ナレッジ運用 |
| 向いている利用者 | まず限定された範囲で回答品質を確認したいチーム | 複数部署、複数資料セット、運用証跡まで必要なチーム |
| 導入範囲 | 1 つの限定されたナレッジベースから開始 | 複数ナレッジベースまたは複数プロジェクトを想定 |
| 利用環境 | 顧客管理環境。社内ネットワーク、オンプレミス、またはプライベートエッジ環境を想定 | 顧客管理環境。運用・監査・復旧も含めて設計 |
| モデル実行 | 顧客環境に応じてローカルモデル構成を確認 | 顧客環境に応じてローカルモデル構成と運用条件を確認 |
| 対象資料 | マニュアル、規程、FAQ、サポートメモ、案件資料などの選定資料 | SKU A の対象に加え、部署別・プロジェクト別の資料セットを整理 |
| ファイル対応 | テキスト抽出可能な PDF、Markdown、テキスト、CSV、その他文書を優先。スキャン画像や複雑なレイアウトは個別確認 | 同左。複雑な資料構造や前処理が必要な場合は導入設計に含めて確認 |
| ユーザー・部署範囲 | 限定されたチームまたは小さな利用範囲 | 複数チーム、複数部署、複数用途を想定 |
| Web コンソール | 質問、回答、ナレッジ一覧、セッション管理 | SKU A に加え、複数ナレッジ・複数プロジェクト管理、品質確認、運用画面を含む |
| ライセンス境界 | Standard 機能の利用範囲を明確化 | Professional 機能の利用範囲を明確化 |
| 回答品質確認 | 初期検証で回答と根拠を確認 | 品質ダッシュボードや継続的な確認フローを含める |
| 引用・根拠確認 | 回答の元資料を確認できる形を重視 | 回答根拠、確認記録、受け入れ証跡まで扱う |
| 受け入れ成果物 | 初期導入範囲、対象資料、利用フロー、回答確認結果 | SKU A に加え、監査出力、受け入れ証跡、運用記録、バックアップ・復旧確認、品質確認記録 |
| 監査出力 | 標準範囲には含めない。必要な場合は SKU B を推奨 | 含める前提で計画可能 |
| バックアップ・復旧 | 標準範囲には含めない。環境要件として個別確認 | 含める前提で計画可能 |
| 運用支援 | 初期導入と確認を中心に支援 | 導入後の安定化、運用確認、証跡整理まで支援 |
| 認証入口 | 顧客管理の認証入口を前提 | 同左。運用・監査前提でより明確な責任分担が必要 |
| 標準外の扱い | 高度な agent-style automation や完全オフライン構成は標準外 | 同左。必要な場合は個別確認 |

### 選び方

SKU A が向いているケース:

- 最初に 1 つの限定範囲で試したい
- 部署や利用者を限定して始めたい
- まず回答品質と根拠表示を確認したい
- 監査出力やバックアップ・復旧までは初期範囲に入れない

SKU B が向いているケース:

- 複数部署または複数ナレッジベースで使いたい
- 導入後の運用確認まで含めたい
- 受け入れ証跡、監査出力、バックアップ・復旧確認が必要
- 品質確認や運用記録を継続的に扱いたい

### 導入前に確認すること

- どの資料を最初の対象にするか
- 誰が利用するか、どの部署から始めるか
- どの環境で動かすか
- 顧客側の認証入口やネットワーク境界
- 受け入れ時に必要な証跡
- バックアップ、復旧、監査出力、品質確認が必要か
- 完全ローカル要件や特殊な運用条件が必要か

---

## English

### Comparison Table

| Area | SKU A: Standard Private RAG | SKU B: Professional Private RAG |
| --- | --- | --- |
| Purpose | Start with private knowledge Q&A | Support daily operations across multiple knowledge bases or teams |
| Best for | Teams that want to validate answer quality within one bounded scope | Teams that need multi-team use, operational evidence, and stronger delivery support |
| Deployment scope | Starts with one bounded knowledge base | Designed for multiple knowledge bases or projects |
| Runtime environment | Customer-controlled environment on private network, on-premise server, or private edge node | Customer-controlled environment with additional operational, audit, and recovery considerations |
| Model execution | Local model setup is reviewed against the customer environment | Local model setup and operational conditions are reviewed against the customer environment |
| Supported documents | Selected manuals, policies, FAQs, support notes, project records, and similar internal materials | Same as SKU A, with support for organizing department-level or project-level document sets |
| File handling | Prioritizes text-readable PDFs, Markdown, text files, CSV, and other extractable documents. Scanned images and complex layouts are reviewed case by case | Same as SKU A. Complex preprocessing needs are handled during delivery scoping |
| Users / departments | Limited team or bounded first-use group | Multiple teams, departments, or use cases |
| Web console | Q&A, answer review, knowledge catalog, and sessions | SKU A plus multi-knowledge-base / multi-project management, quality review, and operational surfaces |
| License boundary | Standard feature boundary | Professional feature boundary |
| Answer-quality review | Initial answer and source review | Quality dashboard and recurring quality-review flow are in scope |
| Citations / evidence | Focuses on reviewable source references | Extends into acceptance evidence and operational records |
| Acceptance deliverables | Initial scope, document boundary, usage flow, and answer-review results | SKU A plus audit export, acceptance evidence, operational records, backup/restore checks, and quality review records |
| Audit export | Not part of the standard scope. Use SKU B if needed | Can be planned as part of the package |
| Backup / restore | Not part of the standard scope. Confirm as an environment requirement if needed | Can be planned as part of the package |
| Operations support | Focused on initial setup and validation | Includes stronger stabilization, operational review, and evidence preparation |
| Authentication ingress | Customer-controlled ingress is assumed | Same, with clearer operational ownership for audit and day-2 operations |
| Out of standard scope | Advanced agent-style automation and fully offline delivery are out of scope | Same. These require separate confirmation |

### How to Choose

Choose SKU A if:

- You want to start with one bounded project or knowledge base
- You want a limited pilot group or team
- You mainly need to validate answer quality and source review
- Audit export and backup/restore checks are not part of the initial scope

Choose SKU B if:

- You need multiple teams, projects, or knowledge bases
- You want operational readiness support after initial setup
- You need acceptance evidence, audit export, or backup/restore checks
- You want recurring quality review and operational records

### What To Confirm Before Delivery

- First document set and knowledge-base boundary
- Initial users, teams, or departments
- Runtime environment
- Customer authentication ingress and network boundary
- Acceptance evidence required before rollout
- Whether audit export, backup, restore, or quality review are required
- Whether fully local-only or unusual operating constraints must be enforced
