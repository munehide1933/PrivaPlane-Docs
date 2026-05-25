# Deployment Options

**Current deployment options and runtime assumptions for PrivaPlane.**  
**PrivaPlane の現時点での導入方式と実行前提を整理した資料です。**

---

## 日本語

### 提供方針（現時点）

PrivaPlane は、**顧客管理環境へのローカル交付**を基本方針としています。  
公開 SaaS に一気に寄せるのではなく、対象資料・利用者・運用範囲を確認しながら導入します。

### 導入オプション

| オプション | 概要 | 向いているケース | 事前確認事項 |
| --- | --- | --- | --- |
| A. MacBook / Mac Studio（ローカル実行） | 顧客側 Mac 環境で 7B-14B クラスのモデルを実行 | 少人数の部門導入、現場デモ、短期間検証 | メモリ容量、チップ世代、同時利用人数、期待応答速度 |
| B. 顧客自備 GPU Linux サーバー | 顧客の GPU サーバー上に構成し運用 | 複数利用者、長時間運用、応答性能重視 | GPU 種別/VRAM、OS、ネットワーク境界、運用担当体制 |
| C. CPU-only 実行（限定運用） | GPU なし環境で実行。機能確認は可能 | 初期検証、機能確認、限定ユーザー | 応答遅延の許容、モデルサイズ調整、同時アクセス制限 |

### 7B-14B モデルについて

- MacBook / Mac Studio で 7B-14B クラスを動かす構成は、顧客環境に応じて確認可能です。  
- ただし、全ての端末で同一性能を保証するものではありません。  
- 実運用可否は、メモリ、量子化方式、同時利用、期待レイテンシで判断します。

### CPU-only の扱い

- CPU-only でも動作検証や限定利用は可能です。  
- ただし、GPU 構成と比べて応答速度や同時処理性能は下がります。  
- 商用運用での快適性は、対象業務と許容待ち時間に応じて事前評価が必要です。

### 導入前チェックリスト

1. 対象資料の種類と量（初期範囲）  
2. 想定ユーザー数と同時利用の有無  
3. 必要な応答速度（業務許容値）  
4. 運用担当者の有無（監視・バックアップ・障害対応）  
5. 受け入れ時に必要な証跡（回答例、引用根拠、運用記録）

---

## English

### Delivery Policy (Current)

PrivaPlane is currently delivered into a **customer-controlled local environment**.  
The rollout starts with a bounded scope instead of forcing a full public SaaS migration.

### Deployment Options

| Option | Summary | Best fit | Pre-check items |
| --- | --- | --- | --- |
| A. MacBook / Mac Studio (local runtime) | Run 7B-14B class models on customer-managed Mac hardware | Small-team rollout, onsite demo, fast pilot | Memory size, chip generation, concurrency, target response speed |
| B. Customer-provided GPU Linux server | Deploy and run on customer GPU Linux environment | Multi-user usage, longer operation windows, performance-oriented teams | GPU type/VRAM, OS, network boundary, operational ownership |
| C. CPU-only runtime (limited mode) | Operate without GPU; valid for functional checks | Initial validation, limited-user pilot | Latency tolerance, model sizing, concurrency limits |

### About 7B-14B on Mac

- A 7B-14B local model path on MacBook or Mac Studio can be reviewed and confirmed case by case.  
- This is not a promise of identical performance on every device.  
- Practical feasibility depends on memory, quantization strategy, concurrency, and latency target.

### CPU-only Positioning

- CPU-only can be used for validation and limited usage.  
- Response speed and throughput are generally lower than GPU setups.  
- Commercial usability should be evaluated against actual workflow and wait-time tolerance.

### Pre-Delivery Checklist

1. Initial document boundary (type and volume)  
2. Expected user count and concurrency  
3. Required response speed for daily operations  
4. Operational owner for monitoring, backup, and incident response  
5. Acceptance evidence needs (answer samples, citations, operational records)
