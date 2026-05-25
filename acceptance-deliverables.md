# Acceptance Deliverables

**What customers receive at acceptance and handover.**  
**導入受け入れ時に、顧客へ何を交付するかを整理した資料です。**

---

## 日本語

### この資料の目的

購買・導入担当が最も気にする「買った後に何が残るか」を明確にします。  
ここでは、標準交付物と条件付き交付物を分けて記載します。

### 標準交付物（SKU A / SKU B 共通）

| 交付物 | 内容 | 形式 |
| --- | --- | --- |
| 環境構成サマリー | 導入対象環境、主要コンポーネント、前提条件 | Markdown / PDF |
| 対象資料一覧 | 初期取り込み対象の資料範囲、除外範囲、版情報 | Markdown / CSV |
| 受け入れ質問セット | 導入時に確認する質問一覧（業務質問、境界質問） | Markdown |
| 回答サンプル | 受け入れ質問に対する回答例 | Markdown / JSON |
| 引用・根拠確認例 | 回答に対する参照文書名・該当箇所の確認例 | Markdown |
| 操作・運用メモ | 利用開始時の基本操作、運用上の注意点 | Markdown |

### 条件付き交付物（主に SKU B）

| 交付物 | 内容 | 想定条件 |
| --- | --- | --- |
| 監査出力サンプル | 利用記録や確認記録の出力例 | 監査要件がある場合 |
| バックアップ手順 | バックアップ対象、実行手順、保管方針 | バックアップ要件がある場合 |
| 復旧確認記録 | 復旧手順と確認結果 | 復旧検証を契約範囲に含む場合 |
| 運用安定化チェック | 初期運用での確認項目と改善メモ | 継続運用支援を含む場合 |

### 受け入れ判定の最低ライン（例）

1. 指定した質問セットに対して、回答と根拠確認ができる  
2. 対象資料の範囲が明確で、除外範囲も合意されている  
3. 利用開始に必要な運用メモが引き渡されている  
4. （必要時）監査・バックアップ・復旧関連の証跡が確認できる

### 注意事項

- 交付物の粒度は、顧客の監査要件・運用要件に合わせて調整します。  
- 全顧客に同一フォーマットを固定提供するのではなく、受け入れ条件に沿って確定します。

---

## English

### Purpose

This document clarifies what the customer receives after purchase and acceptance.  
Deliverables are split into standard and conditional items.

### Standard Deliverables (Common to SKU A / SKU B)

| Deliverable | Description | Format |
| --- | --- | --- |
| Environment summary | Deployment target, major components, and assumptions | Markdown / PDF |
| Document scope list | In-scope and out-of-scope document boundary with version notes | Markdown / CSV |
| Acceptance question set | Questions used for acceptance (business and boundary checks) | Markdown |
| Answer samples | Sample answers for acceptance questions | Markdown / JSON |
| Citation/evidence samples | Source file and relevant passage examples for answer verification | Markdown |
| Operations handover note | Basic usage and operational cautions for go-live | Markdown |

### Conditional Deliverables (Mostly SKU B)

| Deliverable | Description | Typical condition |
| --- | --- | --- |
| Audit export samples | Example exports for usage/review records | When audit requirements exist |
| Backup procedure | Backup scope, run steps, and retention approach | When backup requirements exist |
| Restore validation record | Recovery steps and validation results | When restore checks are in project scope |
| Operational stabilization checklist | Early operation checkpoints and improvement notes | When post-go-live support is included |

### Minimum Acceptance Baseline (Example)

1. Agreed question set can be answered with reviewable evidence  
2. Document boundary (including exclusions) is explicit  
3. Handover notes required for start of operation are delivered  
4. If required, audit/backup/restore evidence is verifiable

### Notes

- Deliverable depth is adjusted to customer audit and operation requirements.  
- Exact format is finalized against acceptance conditions, not forced as one fixed template for every customer.
