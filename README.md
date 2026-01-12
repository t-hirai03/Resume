# 職務経歴書

## 基本情報

| 項目 | 内容 |
|------|------|
| 氏名 | 平井 隆裕 |
| 生年月日 | 1995年9月23日 |
| 居住地 | 神奈川県 |

## 職務要約

Webエンジニアとして、フロントエンドからインフラまで幅広く担当。現職では約1年間で6サイトの保守・5プロジェクトを推進し、PR 186件を達成。GitHub Actions による CI/CD 構築、Terraform/GCP によるデータ基盤構築など、未経験技術も積極的にキャッチアップしながら業務効率化・自動化を推進。

## スキル

| カテゴリ | スキル |
|----------|--------|
| フロントエンド | React, Next.js, Astro, TypeScript, Tailwind CSS, Radix UI |
| バックエンド | Node.js, Supabase (PostgreSQL), Rails (フロント部分) |
| インフラ | Terraform/Terragrunt, GCP (BigQuery, Cloud Run, Cloud SQL, Secret Manager), Docker |
| CI/CD | GitHub Actions, キーレス認証 (Workload Identity Federation) |
| その他 | WordPress, microCMS, Playwright, Google Maps API |

## 職務経歴

### 株式会社シーラ（2024年1月〜現在）　※現職

不動産投資・クラウドファンディング事業を展開する企業のIT部門にて、Webエンジニアとして勤務。

#### プロジェクト1: rimawarikun（利回りくん）

不動産クラウドファンディング投資サービスのフロントエンド開発。

| 項目 | 内容 |
|------|------|
| 役割 | フロントエンドエンジニア（フロントは自分のみ） |
| 技術 | Rails（フロント・バック一体型）、Next.js |
| 担当 | 会員登録・完了画面・マイページのUI改善、キャンペーン用LP 6ページ制作、デザインシステム構築の提案 |

**状況・課題:**
- Next.jsでのフロント切り分けリニューアルの話が出ていたが進んでいなかった
- デザインシステムが未整備で、コンポーネントの一貫性がなかった

**行動・判断:**
- デザインシステムの重要性を認識し、自ら提案（PR#390）
- 他部署案件でNext.jsを使い、小規模案件から導入を進めた

**成果:**
- rimawarikun関連PR: 27件
- サービスURL: https://rimawarikun.com/

---

#### プロジェクト2: starpaint（スターペイント）

塗装会社のWebサイト群（コーポレート・マガジン・フランチャイズLP）の開発・改修。

| 項目 | 内容 |
|------|------|
| 役割 | コーディング担当（一人） |
| 技術 | WordPress, Next.js |
| 担当 | HP改修、マガジンサイト改修、フランチャイズLP改修、チャットボット作成、Chatwork/Notion連携 |

**状況・課題:**
- お問い合わせがあっても見逃すことがあった
- どのURLから流入したか把握できていなかった

**行動・判断:**
- 自ら設計・提案してChatwork/Notion連携を実装
- チャットボット（塗装見積もり→電話番号入力→リード獲得）をNext.jsで設計・開発

**成果:**
- 自作チャットボットで**月間約40件のリード獲得**に貢献（CPA約13,000円で安定稼働）
- Chatwork通知連携でお問い合わせの見逃し防止
- 流入経路の把握を可能に
- チャットボットURL: https://estimate.starpaint.jp/ / https://estimate.starpaint.jp/subsidy/
- サイトURL: https://starpaint.jp/ / https://magazine.starpaint.jp/ / https://fc.starpaint.jp/

---

#### プロジェクト3: WordPress開発環境の近代化

4つのWordPressサイト（syla-holdings、starpaint 3サイト）の開発・運用環境を構築。

| 項目 | 内容 |
|------|------|
| 役割 | 一人で構築・導入 |
| 技術 | WordPress, GitHub, GitHub Actions, Local |

**状況・課題:**
- 6サイトを一人で保守する体制で作業時間の確保が課題
- WordPress管理画面の外観エディタでコーディングしていた
- 本番に直接アップロードして確認する運用
- 1回の更新に5〜10分の手動FTP作業（ログイン→バックアップ→アップロード）

**行動・判断:**
- 既存サイトをGitHubリポジトリ化
- GitHub Actionsで自動FTPデプロイを構築
- Localでローカル開発環境を整備
- 管理画面コーディングからエディタ+Git運用に移行

**成果:**
- 月50〜100分の手動作業削減（月10回更新 × 5〜10分）
- 本番前にローカルで検証可能に
- PR作成→マージで更新完了する運用に
- サイトURL: https://syla-holdings.jp/ / https://syla.jp/ / https://syla-solar.jp/

---

#### プロジェクト4: syla-properties-map（物件マップ）

不動産物件をGoogle Maps上にインタラクティブに表示するWebアプリ。コーポレートサイトにiframeで埋め込み。

| 項目 | 内容 |
|------|------|
| 役割 | 一人でフルスタック開発 |
| 技術 | Astro, React 19, TypeScript, Supabase, Google Maps API, Vercel |
| 担当 | マップ表示、フィルタリング機能、管理画面（CRUD）、画像アップロード |

**状況・課題:**
- 既存のWordPressサイトに物件マップを追加する要件
- WordPress本体に組み込むとパフォーマンス低下、プラグイン依存、保守リスクが発生

**行動・判断:**
- WordPressではなく独立アプリとして開発し、iframeで疎結合に
- Astroのアイランドアーキテクチャで必要な部分だけReact化（パフォーマンス重視）
- Supabaseで管理画面のバックエンドを実装

**成果:**
- 約2〜3週間でMVP開発
- 200件の物件データに対応
- 47ファイルのTypeScript/React/Astroコードを実装
- サービスURL: https://syla-properties-map.vercel.app/

---

#### プロジェクト5: syla-infra（データ統合基盤）

外部SaaS（ieLove：物件管理システム）のデータをBigQueryに集約するデータ統合基盤。

| 項目 | 内容 |
|------|------|
| 役割 | 一人でインフラ・アプリ・CI/CD全て構築 |
| 技術 | Terraform/Terragrunt, GCP (BigQuery, Cloud Run, Cloud SQL), TypeScript, Playwright, Docker, GitHub Actions |

**状況・課題:**
- 賃貸契約データがieLove（外部SaaS）に閉じており、全社横断の分析・活用が困難
- データ取得・変換・格納の自動化が求められていた

**行動・判断:**
- 未経験のTerraform/BigQuery/Cloud Runを触りながらキャッチアップ
- Playwrightで認証付きサイトからCSV自動取得
- CI/CDは安全性・可視性を重視して設計
  - PRへのTerraform Plan自動投稿（レビュー効率化）
  - 確認入力必須デプロイ（誤操作防止）
  - キーレス認証（セキュリティ強化）

**成果:**
- 毎日9時にETL実行→10時にDB同期が自動稼働
- 3種類のCSV（123列+拡張予定+23列）を18テーブルに正規化
- Terraform 3,200行 + アプリ 18,800行
- Dockerイメージ 2.9GB → 875MBに削減（70%減）

---

### 株式会社ジェイクール（2022年1月〜2023年12月）

Web制作・Web更新代行サービスを提供する企業にて、Webエンジニアとして勤務。

| 項目 | 内容 |
|------|------|
| 事業内容 | Web制作、Web更新代行 |
| 役割 | Webサイト制作、Webサイト更新代行 |
| 技術 | WordPress, Astro |

**制作実績（9サイト）:**
- https://kait-ext.securesite.jp/company/index.html
- https://jgi-inc.com/
- https://beyerdynamic.co.jp/
- https://karayasankyo.com/
- https://tg-misawawork.sakura.ne.jp/nasuworkation/
- https://chunichi-chishitsu.com/
- https://kaneki-unyu.co.jp/
- https://obataseishijo.jp/lp/
- https://takazen-sangyo.com/

---

### 株式会社パワーシステム（2018年4月〜2021年10月）

SES企業にて、フロントエンド・バックエンドエンジニアとして勤務。

| 項目 | 内容 |
|------|------|
| 事業内容 | SES |
| 役割 | フロントエンド・バックエンド開発、仕様書作成 |
| 技術 | Vue.js, Java, PostgreSQL |
| 主な案件 | 福井県民衛星プロジェクト |

---

## 自己PR

| 強み | 根拠となる実績 |
|------|----------------|
| 幅広い技術領域をカバーできる | フロントエンド〜インフラまで対応、6サイトの保守を担当 |
| 未経験技術へのキャッチアップ力 | Terraform/BigQuery/Cloud Runを触りながら習得 |
| 効率化・自動化への意識 | FTP手動→GitHub Actions、ETL自動化で月50〜100分削減 |
| 設計判断力 | WordPress vs 独立アプリ、疎結合設計の選択 |
| セキュリティ意識 | キーレス認証、Secret Manager、確認入力必須デプロイ |
