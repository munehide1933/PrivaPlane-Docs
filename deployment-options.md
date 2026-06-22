# Deployment Options

**Current delivery paths and deployment assumptions for PrivaPlane.**  
**PrivaPlane の現時点での導入方式と実行前提を整理した資料です。**

---

## 日本語

### 提供方針（現時点）

PrivaPlane は、**顧客管理環境への導入**を基本方針としています。  
公開 SaaS に一気に寄せるのではなく、対象資料・利用者・運用範囲・認証入口を確認しながら導入します。

標準的には、顧客管理環境に合わせたパッケージ交付と導入支援を前提に進めます。完全オフライン要件や特殊な運用条件がある場合は、最初の確認段階で扱います。

### 導入オプション

| オプション | 概要 | 向いているケース | 事前確認事項 |
| --- | --- | --- | --- |
| A. 顧客管理 Mac ホスト | 顧客側 Mac 環境で構成し運用 | 少人数の部門導入、現場デモ、短期間検証 | メモリ容量、チップ世代、同時利用人数、期待応答速度 |
| B. 顧客自備 GPU Linux サーバー | 顧客の GPU サーバー上に構成し運用 | 複数利用者、長時間運用、応答性能重視 | GPU 種別/VRAM、OS、ネットワーク境界、認証入口、運用担当体制 |
| C. CPU-only 実行（限定運用） | GPU なし環境で実行。機能確認や限定運用向け | 初期検証、機能確認、限定ユーザー | 応答遅延の許容、モデルサイズ調整、同時アクセス制限 |

### ローカルモデル実行について

- MacBook / Mac Studio で 7B-14B クラスを使う構成は、顧客環境に応じて確認します。  
- すべての端末で同一性能を保証するものではありません。  
- 実運用可否は、メモリ、量子化方式、同時利用、期待レイテンシで判断します。

### 外部連携の扱い

- 顧客管理環境への導入を前提としますが、必要な連携先や運用条件は案件ごとに確認します。  
- 「顧客管理環境に導入する」ことと、「一切の外部サービスを使わない」ことは同義ではありません。  
- 完全ローカル運用や air-gapped 要件が必要な場合は、標準説明ではなく別途スコープ確認が必要です。

### CPU-only の扱い

- CPU-only でも動作検証や限定利用は可能です。  
- ただし、GPU 構成と比べて応答速度や同時処理性能は下がります。  
- 商用運用での快適性は、対象業務と許容待ち時間に応じて事前評価が必要です。

### 導入前チェックリスト

1. 対象資料の種類と量（初期範囲）  
2. 想定ユーザー数と同時利用の有無  
3. 必要な応答速度（業務許容値）  
4. 顧客側の認証入口とアクセス制御の置き方  
5. 運用担当者の有無（監視・バックアップ・障害対応）  
6. 完全ローカル要件や特殊なネットワーク制約の有無  
7. 受け入れ時に必要な証跡（回答例、引用根拠、運用記録）

---

## English

### Delivery Policy (Current)

PrivaPlane is currently delivered into a **customer-controlled environment**.  
The rollout starts with a bounded scope instead of forcing a full public SaaS migration.

The standard path is a guided package handoff into the customer-managed environment. Fully offline requirements or unusual operational constraints should be confirmed during scoping.

### Deployment Options

| Option | Summary | Best fit | Pre-check items |
| --- | --- | --- | --- |
| A. Customer-managed Mac host | Deploy and operate on customer-managed Mac hardware | Small-team rollout, onsite demo, fast pilot | Memory size, chip generation, concurrency, target response speed |
| B. Customer-provided GPU Linux server | Deploy and operate on customer GPU Linux | Multi-user usage, longer operation windows, performance-oriented teams | GPU type/VRAM, OS, network boundary, authentication ingress, operational ownership |
| C. CPU-only runtime (limited mode) | Operate without GPU for validation or limited usage | Initial validation, limited-user pilot | Latency tolerance, model sizing, concurrency limits |

### Local Model Runtime

- A 7B-14B model path on MacBook or Mac Studio can be reviewed case by case.  
- This is not a promise of identical performance on every device.  
- Practical feasibility depends on memory, quantization strategy, concurrency, and latency target.

### External Dependency Position

- The deployment is customer-controlled, but any needed integrations or connectivity assumptions should still be confirmed case by case.  
- Therefore, "customer-controlled deployment" should not be read as a blanket promise that no external service is ever involved.  
- If fully local-only or air-gapped operation is required, it should be scoped explicitly instead of assumed as the default baseline.

### CPU-only Positioning

- CPU-only can be used for validation and limited usage.  
- Response speed and throughput are generally lower than GPU setups.  
- Commercial usability should be evaluated against actual workflow and wait-time tolerance.

### Pre-Delivery Checklist

1. Initial document boundary (type and volume)  
2. Expected user count and concurrency  
3. Required response speed for daily operations  
4. Customer authentication ingress and access-control boundary  
5. Operational owner for monitoring, backup, and incident response  
6. Whether fully local-only or unusual network constraints apply  
7. Acceptance evidence needs (answer samples, citations, operational records)
