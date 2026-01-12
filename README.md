# 職務経歴書

2026年1月12日現在
氏名：平井 隆裕

## 概要

Webエンジニアとして、フロントエンドからインフラまで幅広く担当。現職では約1年間で6サイトの保守・5プロジェクトを推進し、PR 186件を達成。GitHub Actions による CI/CD 構築、Terraform/GCP によるデータ基盤構築など、未経験技術も積極的にキャッチアップしながら業務効率化・自動化を推進。

## 技術スキル / ソフトスキル

### 技術スキル

- **フロントエンド:** React, Next.js, Astro, TypeScript, Tailwind CSS, Radix UI
- **バックエンド:** Node.js, Supabase (PostgreSQL), Rails（モノリシック構成でのフロントエンド開発経験）
- **インフラ:** Terraform/Terragrunt, GCP (BigQuery, Cloud Run, Cloud SQL, Secret Manager), Docker
- **CI/CD:** GitHub Actions, キーレス認証 (Workload Identity Federation)
- **その他:** WordPress, microCMS, Playwright, Google Maps API

### ソフトスキル

- **未経験技術へのキャッチアップ力:** Terraform/BigQuery/Cloud Runを触りながら習得
- **効率化・自動化への意識:** FTP手動→GitHub Actions、ETL自動化で月50〜100分削減
- **設計判断力:** WordPress vs 独立アプリ、疎結合設計の選択

## 職務経歴

### 株式会社シーラ　2024年1月〜現在

事業内容：不動産投資・クラウドファンディング事業

#### 代表的なプロジェクト

| 期間 | プロジェクト |
|------|-------------|
| 2024年1月〜現在 | rimawarikun（利回りくん） |
| 2024年1月〜現在 | starpaint（スターペイント） |
| 2024年1月〜現在 | WordPress開発環境の近代化 |
| 2024年9月〜現在 | syla-properties-map（物件マップ） |
| 2024年6月〜現在 | syla-infra（データ統合基盤） |

---

#### rimawarikun（利回りくん）

不動産クラウドファンディング投資サービスのフロントエンド開発。

**チーム構成:** フロントエンド 1名（自分のみ）、バックエンド 2名

**使用技術:** Rails（フロント・バック一体型）、Next.js

**自身の担当業務:**
- 会員登録・完了画面・マイページのUI改善
- キャンペーン用LP 6ページ制作
- デザインシステム構築の提案

**状況・課題 / 工夫した取り組み / 成果:**
- Next.jsでのフロント切り分けリニューアルの話が出ていたが進んでいなかった
- デザインシステムの重要性を認識し、自ら提案（PR#390）
- 他部署案件でNext.jsを使い、小規模案件から導入を進めた
- rimawarikun関連PR: 27件

**URL:** https://rimawarikun.com/

---

#### starpaint（スターペイント）

塗装会社のWebサイト群（コーポレート・マガジン・フランチャイズLP）の開発・改修。

**チーム構成:** コーディング担当 1名（自分のみ）

**使用技術:** WordPress, Next.js

**自身の担当業務:**
- HP改修、マガジンサイト改修、フランチャイズLP改修
- チャットボット作成
- Chatwork/Notion連携

**状況・課題 / 工夫した取り組み / 成果:**
- お問い合わせがあっても見逃すことがあった
- 自ら設計・提案してChatwork/Notion連携を実装
- チャットボット（塗装見積もり→電話番号入力→リード獲得）をNext.jsで設計・開発
- 自作チャットボットで**月間約40件のリード獲得**に貢献（CPA約13,000円で安定稼働）
- Chatwork通知連携でお問い合わせの見逃し防止

**URL:**
- チャットボット: https://estimate.starpaint.jp/ / https://estimate.starpaint.jp/subsidy/
- サイト: https://starpaint.jp/ / https://magazine.starpaint.jp/ / https://fc.starpaint.jp/

---

#### WordPress開発環境の近代化

4つのWordPressサイト（syla-holdings、starpaint 3サイト）の開発・運用環境を構築。

**チーム構成:** 1名（自分のみ）

**使用技術:** WordPress, GitHub, GitHub Actions, Local

**自身の担当業務:**
- 既存サイトのGitHubリポジトリ化
- GitHub Actionsで自動FTPデプロイを構築
- Localでローカル開発環境を整備

**状況・課題 / 工夫した取り組み / 成果:**
- 6サイトを一人で保守する体制で作業時間の確保が課題
- WordPress管理画面の外観エディタでコーディング→本番直接アップロードの運用だった
- 月50〜100分の手動作業削減（月10回更新 × 5〜10分）
- 本番前にローカルで検証可能に
- PR作成→マージで更新完了する運用に

**URL:** https://syla-holdings.jp/ / https://syla.jp/ / https://syla-solar.jp/

---

#### syla-properties-map（物件マップ）

不動産物件をGoogle Maps上にインタラクティブに表示するWebアプリ。コーポレートサイトにiframeで埋め込み。

**チーム構成:** 1名（自分のみ）

**使用技術:** Astro, React 19, TypeScript, Supabase, Google Maps API, Vercel

**自身の担当業務:**
- マップ表示、フィルタリング機能
- 管理画面（CRUD）、画像アップロード

**状況・課題 / 工夫した取り組み / 成果:**
- 既存のWordPressサイトに物件マップを追加する要件
- WordPress本体に組み込むとパフォーマンス低下、プラグイン依存、保守リスクが発生
- WordPressではなく独立アプリとして開発し、iframeで疎結合に
- Astroのアイランドアーキテクチャで必要な部分だけReact化（パフォーマンス重視）
- 200件の物件データに対応、47ファイルのコードを実装

**URL:** https://syla-properties-map.vercel.app/

---

#### syla-infra（データ統合基盤）

外部SaaS（ieLove：物件管理システム）のデータをBigQueryに集約するデータ統合基盤。

**チーム構成:** 1名（自分のみ）

**使用技術:** Terraform/Terragrunt, GCP (BigQuery, Cloud Run, Cloud SQL), TypeScript, Playwright, Docker, GitHub Actions

**自身の担当業務:**
- インフラ・アプリ・CI/CD全て構築
- Playwrightで認証付きサイトからCSV自動取得
- PRへのTerraform Plan自動投稿、確認入力必須デプロイ、キーレス認証

**状況・課題 / 工夫した取り組み / 成果:**
- 賃貸契約データがieLove（外部SaaS）に閉じており、全社横断の分析・活用が困難
- 未経験のTerraform/BigQuery/Cloud Runを触りながらキャッチアップ
- 毎日9時にETL実行→10時にDB同期が自動稼働
- 3種類のCSV（123列+拡張予定+23列）を18テーブルに正規化
- Terraform 3,200行 + アプリ 18,800行
- Dockerイメージ 2.9GB → 875MBに削減（70%減）

---

### 株式会社ジェイクール　2022年1月〜2023年12月

事業内容：Web制作、Web更新代行

**役割:** Webサイト制作、Webサイト更新代行

**使用技術:** WordPress, Astro

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

### 株式会社パワーシステム　2018年4月〜2021年10月

事業内容：SES

**役割:** フロントエンド・バックエンド開発、仕様書作成

**使用技術:** Vue.js, Java, PostgreSQL

**主な案件:** 福井県民衛星プロジェクト

---

## スキル

| カテゴリ | 技術・ツール | 経験年数 |
|----------|-------------|----------|
| 言語 | TypeScript, JavaScript | 3年 |
| 言語 | Java | 3年 |
| FW & ライブラリ | React, Next.js | 2年 |
| FW & ライブラリ | Astro | 1年 |
| FW & ライブラリ | Vue.js | 2年 |
| インフラ・クラウド | GCP (BigQuery, Cloud Run), Docker, Terraform | 1年 |
| CMS | WordPress | 4年 |
| 開発プロセス | GitHub Actions, CI/CD | 2年 |

## アウトプット

- **GitHub:** https://github.com/t-hirai03

## 学歴

- 神奈川工科大学 情報学部 情報工学科（2018年3月卒業）
