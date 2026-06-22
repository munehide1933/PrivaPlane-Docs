# FAQ for Buyers

**A practical FAQ for PrivaPlane buyers, project owners, and IT reviewers.**  
**PrivaPlane の導入を検討する購買担当者・導入担当者・IT レビュー担当者向け FAQ。**

This FAQ avoids broad security claims and focuses on what can be confirmed during a real delivery discussion.

この FAQ では、抽象的な安全性の宣伝ではなく、実際の導入前に確認できる内容を中心に整理します。

---

## 日本語

### Q1. データは顧客環境の外に出ますか？

PrivaPlane は、顧客が管理できる環境に導入することを前提にしています。典型的には、顧客側の認証入口の背後、社内ネットワーク、オンプレミス環境、またはプライベートエッジ環境で動かす形を想定します。

ただし、「顧客管理環境に導入する」ことと、「一切の外部サービスを使わない」ことは同義ではありません。必要な連携先、送信対象、責任分担、完全ローカル要件の有無は、導入前に明確にします。

完全ローカル運用や air-gapped 要件を必須にする場合は、標準説明ではなく別途の導入条件として確認してください。

### Q2. 顧客データをモデル学習に使いますか？

標準の PrivaPlane は、顧客資料をもとに検索・参照して回答する RAG 型の利用を前提にしています。顧客データをモデル学習に利用することは標準範囲ではありません。

ファインチューニングや追加学習が必要な場合は、別途合意、対象データ、目的、保存範囲、削除方法を確認する必要があります。

### Q3. どのような資料に対応できますか？

最初は、テキスト抽出しやすい資料から始めることを推奨します。

想定する資料:

- 社内マニュアル
- 規程、手順書、業務ルール
- FAQ、問い合わせ履歴、サポートメモ
- 議事録、案件資料、プロジェクト記録
- CSV、Markdown、テキスト、テキスト抽出可能な PDF

スキャン画像、手書き資料、表が多い複雑な PDF、画像中心の資料は、OCR や前処理が必要になる場合があります。正式な対応範囲は、最初の資料確認時に判断します。

### Q4. 導入にはどれくらい時間がかかりますか？

固定の日数は、資料量、環境準備、確認フロー、顧客側レビュー体制によって変わります。PrivaPlane は、最初から全社展開するよりも、小さな資料セットで検証してから広げる進め方を推奨しています。

基本の流れ:

1. 対象資料、利用者、環境、受け入れ条件を確認する。
2. 顧客管理環境に合わせて準備する。
3. 最初の資料を取り込み、回答品質と根拠表示を確認する。
4. 受け入れ証跡を整理し、次の展開範囲を決める。

### Q5. 顧客側で何を用意する必要がありますか？

導入前に、以下を確認できると進めやすくなります。

- 最初に扱う資料セット
- 利用予定者または検証担当者
- 実行環境。例: Mac ホスト、GPU 搭載 Linux サーバー、社内ネットワーク上のオンプレミスサーバー、プライベートエッジ環境
- 顧客側の認証入口やアクセス制御の考え方
- 外部接続可否と責任分担
- 受け入れ時に確認したい質問例
- 運用上必要な記録、バックアップ、復旧、監査出力の要否

### Q6. SKU A と SKU B の違いは何ですか？

SKU A は、限定された資料範囲から社内資料 Q&A を始めるための基本プランです。まず回答品質、根拠表示、利用フローを確認したい場合に向いています。

SKU B は、複数部署や複数ナレッジベースでの利用、品質確認、監査・受け入れ証跡、バックアップ・復旧確認、運用支援まで含めたい場合に向いています。

詳しくは [SKU A/B Comparison](./sku-a-b-comparison.md) を参照してください。

### Q7. 監査出力やバックアップ・復旧は含まれますか？

SKU A の標準範囲には含めません。必要な場合は SKU B を推奨します。

SKU B では、監査出力、受け入れ証跡、バックアップ・復旧確認、品質確認、運用記録を含めて検討できます。ただし、具体的な出力項目や復旧手順は顧客環境に合わせて確認します。

### Q8. 顧客ローカル環境への交付や Mac / Linux サーバーでの実行はできますか？

現在の設計では、PrivaPlane は顧客管理環境へ交付し、その環境内で動かす形を重視しています。候補環境としては、Mac ホスト上での構成、または顧客が用意する GPU 搭載 Linux サーバー上で動かす構成を確認できます。

実際の可否や快適に使える範囲は、端末のメモリ、チップ世代、GPU、選択するモデル、量子化方式、同時利用人数、期待する応答速度によって変わります。そのため、導入前に「どの端末で、どのモデルを、どの資料量・利用人数で使うか」を確認します。

この説明は、すべての Mac やすべての 7B〜14B モデルで同じ性能を保証するものではありません。顧客環境に合わせて、実現可能な構成を確認する前提です。

なお、完全オフラインの Mac 交付は、現時点では標準の SKU A / SKU B パッケージ前提ではなく、個別確認の対象です。

### Q9. 導入後に対象資料や部署を増やせますか？

はい。ただし、最初から全範囲を入れるのではなく、最初の資料セットで回答品質と運用方法を確認し、その後に対象を広げる進め方を推奨します。

複数部署や複数ナレッジベースを前提にする場合は、SKU B の範囲として整理する方が自然です。

### Q10. PrivaPlane は汎用チャットボットですか？

いいえ。PrivaPlane は、社内資料をもとに回答し、根拠を確認しながら業務利用するための Private RAG プロダクトです。会話体験そのものよりも、資料境界、回答根拠、導入範囲、運用証跡を重視します。

### Q11. エージェント型自動化や hybrid 実行は標準機能ですか？

いいえ。より高度な agent-style automation や hybrid 実行は、現時点では標準の SKU A / SKU B 説明には含めません。

---

## English

### Q1. Does customer data leave the customer environment?

PrivaPlane is designed to be delivered into a customer-controlled environment. A typical deployment runs behind customer-controlled authentication ingress on a private network, on-premise server, or private edge node.

However, "customer-controlled deployment" should not be read as a blanket promise that no external service is ever involved. Any external integrations, transmitted data scope, responsibility boundary, and fully local-only requirement should be confirmed before delivery.

If fully local or air-gapped operation is mandatory, it should be treated as a separate scoped requirement rather than assumed as the default A/B baseline.

### Q2. Is customer data used to train models?

The standard PrivaPlane usage is RAG-based: it retrieves and references selected customer documents to support answers. Using customer data for model training is not part of the standard scope.

If fine-tuning or additional training is requested, it requires a separate agreement covering target data, purpose, retention, and deletion process.

### Q3. What file types or documents are supported?

The recommended starting point is text-readable documents.

Typical document types:

- Internal manuals
- Policies, procedures, and operating rules
- FAQs, support notes, and inquiry histories
- Meeting notes, project documents, and project records
- CSV, Markdown, text files, and text-extractable PDFs

Scanned images, handwritten documents, complex table-heavy PDFs, and image-centered documents may require OCR or preprocessing. The supported scope is confirmed during the first document review.

### Q4. How long does deployment take?

There is no fixed timeline because the schedule depends on document volume, environment readiness, review process, and customer-side availability. PrivaPlane recommends starting with a bounded document set, validating quality, and then expanding.

Basic flow:

1. Confirm documents, users, environment, and acceptance criteria.
2. Prepare the customer-controlled environment.
3. Ingest the first document set and validate answer quality and source review.
4. Prepare acceptance evidence and decide the next rollout scope.

### Q5. What does the customer need to prepare?

The project can move faster when the following are clear:

- First document set
- Initial users or reviewers
- Runtime environment, such as a Mac host, customer-provided GPU Linux server, on-premise server on a private network, or private edge node
- Authentication ingress and access-control approach
- Whether outbound connectivity is allowed and how responsibility is assigned
- Example questions for acceptance review
- Whether operational records, backup, restore, or audit export are required

### Q6. What is the difference between SKU A and SKU B?

SKU A is the basic package for starting private knowledge Q&A with a bounded document scope. It is suitable when the first goal is to validate answer quality, source review, and usage flow.

SKU B is for teams that need multi-team or multi-knowledge-base use, quality review, audit or acceptance evidence, backup/restore checks, and stronger operational support.

See [SKU A/B Comparison](./sku-a-b-comparison.md) for details.

### Q7. Are audit export and backup/restore included?

They are not part of the standard SKU A scope. If they are required, SKU B is the better fit.

In SKU B, audit export, acceptance evidence, backup/restore checks, quality review, and operational records can be included. The exact outputs and recovery process are confirmed according to the customer environment.

### Q8. Can PrivaPlane be delivered locally and run on Mac or Linux servers?

The current delivery design focuses on handoff into a customer-controlled environment. Candidate runtime environments include a Mac host or a customer-provided Linux server with GPU.

The practical scope depends on device memory, chip generation, GPU availability, selected model, quantization approach, expected concurrency, and target response speed. Before delivery, the runtime plan should confirm which device, which model class, how much document data, and how many users are expected.

This does not mean every Mac or every 7B-14B model will provide the same experience. The intended commitment is that these delivery options can be reviewed and confirmed against the actual customer environment.

Fully offline Mac delivery is not part of the default SKU A / SKU B package assumption today and should be treated as a separately confirmed requirement.

### Q9. Can we expand documents or departments after deployment?

Yes. The recommended approach is to validate the first document set and operating flow before expanding to more documents or departments.

If multiple departments or multiple knowledge bases are expected from the beginning, SKU B is usually the more natural package.

### Q10. Is PrivaPlane a general-purpose chatbot?

No. PrivaPlane is a Private RAG product for answering from internal documents and reviewing the sources behind those answers. It focuses on document boundary, source evidence, delivery scope, and operational records rather than a generic chat interface.

### Q11. Are agent-style automation and hybrid execution standard features?

No. More advanced agent-style automation and hybrid execution are not part of the standard SKU A / SKU B baseline.
