# 職務経歴書

## 基本情報
- 氏名: 中田 恭大
- 居住地: 埼玉県吉川市在住

## 職務経歴
### 株式会社オープンアップITエンジニア
- **在籍期間**: 2021年10月1日から現在に至る

#### 参画プロジェクト: データ伝送システム基盤（AWS）の運用・保守
- **参画期間**: 2023年11月1日から現在
- **概要**
  - AWS基盤の運用保守と継続的な構成改善
  - PCI-DSS 4.0準拠対応: IAMポリシー見直し、暗号化設定、ログ監査、OS/ミドルウェア更新
  - プライベート接続設計: HULFT Squareとオンプレ環境を接続（AWS PrivateLink、Direct Connect、Site-to-Site VPN）
  - 監視自動化: CloudWatch、EventBridge、Lambdaを用いた異常検知・通知・自動リカバリーの仕組みを構築
  - IaCによる構成管理：CloudFormationテンプレートを活用した定型化とドキュメント整備
  - 使用した技術: AWS（EC2, RDS, Lambda, EventBridge, CloudWatch, IAM, S3, CloudFormation）
  - 成果: アラート精度の向上と運用対応負荷の削減を実現し、SLA維持に貢献

#### 参画プロジェクト: データ伝送システムの運用・保守
- **参画期間**: 2021年12月1日から2023年10月31日
- **概要**
  - 新規立ち上げ現場への参画と手順書の作成／改修
  - ISDN回線からIP回線へのデータ伝送方式の切り替えと調整業務
  - EDIを使用したマルチプロトコルでのデータ伝送システムの運用
  - HULFT／全銀TCP/IP／SFTPの三種プロトコルを使用したデータ伝送業務の運用と保守
  - クライアントとの調整業務（電話／メール）
  - Excel VBAを使用したチーム内業務改善（ドキュメント作成等の自動化）
  - データ伝送ログ取得のための簡易的なバッチファイルの作成
  - Linuxコマンド（およびExcel関数）によるログ取得解析

### 株式会社綜合キャリアオプション
- **部署**: 委託事業推進部：官公庁入札案件案担当
- **在籍期間**: 2015年4月1日から2020年3月31日

#### 主な業務内容
- **委託現場管理業務(官公庁担当)**
  - 官公庁案件の入札に関わる現場管理業務を担当。同業他社からのヒアリングを通じて、現場管理や履行体制のノウハウを収集し、提案書の作成に貢献。
  - 人員、工数、納期の管理を含む、200人規模の委託現場の運営に携わり、新人教育や業務フローの改善提案を行い、業務効率の向上に寄与。
  - 官公庁案件の入札プロセスや現場管理における豊富な経験を得るとともに、チームリーダーシップや問題解決能力を養う機会を得ました。

## スキル・技術経験

### プログラミング言語
- Rust（CLI / ログ解析 / TUIツール開発）
- Go（CLIツール試作、API設計学習）
- Python（業務でのLambda自動化やログ処理に使用）

### IaC / 自動化
- AWS CloudFormation（構成テンプレート管理）
- シェルスクリプト（監視・自動化タスク）

### データベース
- Amazon RDS（MySQL / PostgreSQL）
- SQLite（ローカルCLIツール開発で使用）

### コード管理・CI/CD
- Git（GitHubを用いたチーム開発、レビュー・ブランチ管理経験あり）
- GitHub Actions（CI/CDパイプライン構築に活用）

### クラウド・インフラ（AWS）
- AWS全般（3年以上）
  - 運用・自動化: CloudWatch, EventBridge, Lambda, CloudFormation, IAM
  - サーバレス: Lambda, API Gateway, SES
  - ストレージ・配信: S3, CloudFront, Certificate Manager
  - データベース: RDS（MySQL / PostgreSQL）, Aurora
  - ネットワーク: VPC, Direct Connect, PrivateLink, ALB
  - セキュリティ: IAMポリシー, KMS, Secrets Manager, WAF
  - ガバナンス・統制: AWS Organizations, Service Control Policies（SCP）, CloudTrail, Systems Manager

### コンテナ / ミドルウェア
- Docker（ローカル開発環境で使用）
- Apache / Nginx（設定経験あり）

### その他ツール・言語
- Markdown / YAML（ドキュメント・構成管理）
- Shellスクリプト（運用スクリプトの自動化）


## 技術活動・個人開発

- RustやGoを用いたCLIツール・ログ解析ツールなどを個人開発
  - GCログからPause時間を抽出・可視化するツール（RustでCSV出力、Pythonでグラフ描画）
  - Zettelkasten的なメモ管理を支援するTUIツール（現在開発中）
- 開発では「自動化」「可視化」「再現性ある構成」を常に意識し、運用に活かせる知見を蓄積
- GitHub上でのコード公開を通じてアウトプットを継続中

- いずれも「繰り返し作業の削減」「運用の再現性確保」「内省と改善に役立つ仕組みづくり」を重視して設計

- CLI/TUIのUI設計や、構成の可搬性、ログの構造化など、日常の運用改善に直結する技術スタックの探究を継続中

- GitHub上にコードを公開し、ログ分析や構成管理の知見を社外にも還元できるよう努めている

## 開発したシステムやアプリケーションの概要

- インフラ構築・運用の知見を個人開発にも応用し、以下のようなツール・仕組みを実装：

### ログ解析ツール（Rust）
- JavaのG1GCログを解析し、Pause時間の推移をCSV形式に変換
- RustのPlottersクレートを用いて、Pause時間の折れ線グラフを生成
- サービスのメモリ傾向やボトルネック検出に役立つ自動分析ツールとして活用

### ノート管理CLI / TUIツール（Rust）
- Zettelkastenの思想をベースに、Markdown形式でメモを記録・分類・リンク管理
- ReflectやLogなど、思考と行動の記録を助ける構造を実装
- TUI空間で日々の習慣や構想を一元的に扱う「知的作業空間」として開発中

### IaC自動化支援ツール（Rust）
- AWS CloudFormationのYAMLテンプレートをCSVから自動生成するCLIツールを試作中
- サーバレス構成やVPC構成など、反復構成の高速化・誤入力防止を目的に設計

- いずれも「再現性ある運用」「構成の見える化」「改善可能性の確保」を目的に設計・改善を継続

## 学歴
- **最終学歴**: 立教大学
  - 異文化コミュニケーション学部・学科
  - 卒業年月: 2015年03月

## 関連する資格
- ITパスポート
- AWS-SAA (AWS Certified Solutions Architect - Associate)
- AWS-DVA (AWS Certified Developer - Associate)
- AWS-SOA (AWS Certified SysOps Administrator - Associate)
- LPIC 201（202は未取得）

