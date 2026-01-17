# 職務経歴書

2026年1月12日現在
氏名：平井 隆裕

## 概要

一人で事業成果を出すWebエンジニア。現職では6サイトを保守しながら、自作チャットボットで月500万円成約に貢献。未整備な環境をGitHub Actions自動化やTerraform/GCPデータ基盤で立て直し、効率化と事業成果を両立。

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

| 期間 | プロジェクト | 概要 |
|------|-------------|------|
| 2024年1月〜現在 | starpaint | 事業インパクト × 数字 |
| 2024年1月〜現在 | WordPress環境近代化 | 工数削減・運用改善 |
| 2024年6月〜現在 | syla-infra | 未経験技術 × 自走 |

---

#### starpaint（スターペイント）

塗装会社のWebサイト群（コーポレート・マガジン・フランチャイズLP）の開発・改修。

**チーム構成:** コーディング担当 1名（自分のみ）

**使用技術:** WordPress, Next.js

**担当:** Webサイト群の改修およびリード獲得施策の設計・実装

**成果:**
- 自作チャットボットで**月間約50件のリード獲得**、**月3件・約500万円の成約**に貢献
- フランチャイズLP改修で**月15〜20件のパートナー問い合わせ**を獲得
- Chatwork通知連携でお問い合わせの見逃し防止

**URL:**
- チャットボット: https://estimate.starpaint.jp/ / https://estimate.starpaint.jp/subsidy/
- サイト: https://starpaint.jp/ / https://magazine.starpaint.jp/ / https://fc.starpaint.jp/

---

#### WordPress開発環境の近代化

4つのWordPressサイト（syla-holdings、starpaint 3サイト）の開発・運用環境を構築。

**チーム構成:** 1名（自分のみ）

**使用技術:** WordPress, GitHub, GitHub Actions, Local

**担当:** 既存サイトのGit管理化、GitHub Actions自動デプロイ、ローカル開発環境整備

**成果:**
- GitHub Actions自動デプロイで**年間約13時間の作業削減**
- PHP互換性チェックで**PHP7→8移行を1.5ヶ月→2週間に短縮**

**URL:** https://syla-holdings.jp/ / https://syla.jp/ / https://syla-solar.jp/

---

#### syla-properties-map（物件マップ）

不動産物件をGoogle Maps上に表示するWebアプリ。

**使用技術:** Astro, React, TypeScript, Supabase, Google Maps API

**設計判断:** 既存WordPressに組み込むとパフォーマンス低下・保守リスクが発生するため、独立アプリとしてiframeで疎結合に設計。

---

#### syla-infra（データ統合基盤）

外部SaaS（ieLove：物件管理システム）のデータをBigQueryに集約するデータ統合基盤。

**チーム構成:** 1名（自分のみ）

**使用技術:** Terraform/Terragrunt, GCP (BigQuery, Cloud Run, Cloud SQL), TypeScript, Playwright, Docker, GitHub Actions

**担当:** インフラ・アプリ・CI/CD全て一人で構築

**背景:** 賃貸データがieLove・Salesforceで二重管理され、ステータス不整合が発生

**成果:**
- GCP上にデータ基盤を構築し、3種類のCSV（計258列）を18テーブルに正規化
- 毎日自動でETL→DB同期を稼働
- CI/CD自動化で**年間60〜96時間削減**

---

### 株式会社ジェイクール　2022年1月〜2023年12月

事業内容：Web制作、Web更新代行

**役割:** Webサイト制作、Webサイト更新代行

**使用技術:** WordPress, Astro

**実績:** 7サイトの更新代行と並行して9サイトを制作

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

- 大阪経済法科大学 経済学部 経営学科（2018年3月卒業）
