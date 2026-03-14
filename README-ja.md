# Public APIs リポジトリ（日本語版）

> このリポジトリは [public-apis/public-apis](https://github.com/public-apis/public-apis) の日本語版 Fork です。
> メンテナンスは [gumi-ink](https://github.com/gumi-ink) が行っています。
> 元のリポジトリはコミュニティメンバーと [APILayer](https://apilayer.com/) チームによって手作業で管理されています。

これはインターネット上の無料公開 API を整理したリストで、動物、アニメ、ブロックチェーン、本、ビジネス、カレンダー、暗号通貨、開発ツール、辞書、メール、エンターテイメント、環境、金融、食べ物、ゲーム、地理コーディング、政府、健康、仕事、機械学習、音楽、ニュース、オープンデータ、プログラミング、科学、セキュリティ、ショッピング、SNS、スポーツ、天気など 50 以上のカテゴリーをカバーしています。

---

## 📋 目次

- [プロジェクト概要](#プロジェクト概要)
- [API カテゴリー索引](#api-カテゴリー索引)
- [使い方](#使い方)
- [コントリビューション](#コントリビューション)
- [ライセンス](#ライセンス)

---

## プロジェクト概要

Public APIs プロジェクトは、インターネット上のさまざまな無料公開 API インターフェースを収集・整理したものです。

### 主な特徴

- ✅ **完全無料** - 掲載されているすべての API は無料利用枠があります
- ✅ **手作業で厳選** - 各 API はコミュニティによって手作業で審査されています
- ✅ **情報が充実** - 認証方式、HTTPS 対応、CORS 対応などの重要情報を含みます
- ✅ **継続的に更新** - コミュニティ主導で定期的にメンテナンスされます
- ✅ **分類が明確** - 分野別に分類されており、検索が簡単です

---

## API カテゴリー索引

| カテゴリー | 説明 |
|-----------|------|
| [Animals](#animals) | 動物関連 API（猫、犬、鳥類など） |
| [Anime](#anime) | アニメ、漫画関連 API |
| [Anti-Malware](#anti-malware) | マルウェア対策、セキュリティスキャン API |
| [Art & Design](#art--design) | アートとデザイン API |
| [Authentication & Authorization](#authentication--authorization) | 認証と認可 API |
| [Blockchain](#blockchain) | ブロックチェーン関連 API |
| [Books](#books) | 本、読書関連 API |
| [Business](#business) | ビジネス、企業関連 API |
| [Calendar](#calendar) | カレンダー、時間関連 API |
| [Cloud Storage & File Sharing](#cloud-storage--file-sharing) | クラウドストレージとファイル共有 API |
| [Continuous Integration](#continuous-integration) | 継続的インテグレーション API |
| [Cryptocurrency](#cryptocurrency) | 暗号通貨 API |
| [Currency Exchange](#currency-exchange) | 為替レート API |
| [Data Validation](#data-validation) | データ検証 API |
| [Development](#development) | 開発ツール API |
| [Dictionaries](#dictionaries) | 辞書、辞典 API |
| [Documents & Productivity](#documents--productivity) | ドキュメントと生産性 API |
| [Email](#email) | メール関連 API |
| [Entertainment](#entertainment) | エンターテイメント関連 API |
| [Environment](#environment) | 環境、気候関連 API |
| [Events](#events) | イベント関連 API |
| [Finance](#finance) | 金融関連 API |
| [Food & Drink](#food--drink) | 食べ物、飲み物関連 API |
| [Games & Comics](#games--comics) | ゲームと漫画 API |
| [Geocoding](#geocoding) | ジオコーディング、位置情報 API |
| [Government](#government) | 政府オープンデータ API |
| [Health](#health) | 健康、医療関連 API |
| [Jobs](#jobs) | 仕事、採用 API |
| [Machine Learning](#machine-learning) | 機械学習 API |
| [Music](#music) | 音楽関連 API |
| [News](#news) | ニュース API |
| [Open Data](#open-data) | オープンデータ API |
| [Open Source Projects](#open-source-projects) | オープンソースプロジェクト API |
| [Patent](#patent) | 特許関連 API |
| [Personality](#personality) | 性格診断 API |
| [Phone](#phone) | 電話関連 API |
| [Photography](#photography) | 写真関連 API |
| [Programming](#programming) | プログラミング関連 API |
| [Science & Math](#science--math) | 科学と数学 API |
| [Security](#security) | セキュリティ関連 API |
| [Shopping](#shopping) | ショッピング関連 API |
| [Social](#social) | ソーシャルネットワーク API |
| [Sports & Fitness](#sports--fitness) | スポーツとフィットネス API |
| [Test Data](#test-data) | テストデータ API |
| [Text Analysis](#text-analysis) | テキスト分析 API |
| [Tracking](#tracking) | 追跡 API |
| [Transportation](#transportation) | 交通関連 API |
| [URL Shorteners](#url-shorteners) | URL 短縮サービス API |
| [Vehicle](#vehicle) | 車両関連 API |
| [Video](#video) | 動画関連 API |
| [Weather](#weather) | 天気関連 API |

---

## 使い方

### フィールド説明

各 API エントリーには以下の情報が含まれています：

| フィールド | 説明 | 選択肢 |
|-----------|------|--------|
| **API** | API 名とドキュメントリンク | - |
| **Description** | API の機能説明 | - |
| **Auth** | 認証方式 | `No` / `apiKey` / `OAuth` / `X-Mashape-Key` |
| **HTTPS** | HTTPS 対応 | `Yes` / `No` |
| **CORS** | クロスドメイン対応 | `Yes` / `No` / `Unknown` |

### 認証方式の説明

- **No** - 認証不要、直接呼び出し可能
- **apiKey** - API キー/トークンが必要
- **OAuth** - OAuth 認証に対応
- **X-Mashape-Key** - 特定のリクエストヘッダーが必要

### 使用例

```javascript
// 認証不要の API
fetch('https://api.example.com/data')
  .then(response => response.json())
  .then(data => console.log(data));

// API Key が必要な API
fetch('https://api.example.com/data', {
  headers: {
    'X-Api-Key': 'your-api-key-here'
  }
})
  .then(response => response.json())
  .then(data => console.log(data));
```

---

## コントリビューション

Pull Request を歓迎します！

### 提出規約

1. **API 要件**：無料利用枠があり、有料サービスのマーケティングツールでないこと
2. **フォーマット規約**：テーブル形式に従い、アルファベット順を保つ
3. **情報の完全性**：認証方式、HTTPS、CORS 情報を含める
4. **簡潔な説明**：説明は 100 文字以内
5. **PR タイトル**：`Add API-name API` 形式（例：`Add Weather API`）

### 提出手順

1. このリポジトリを Fork
2. 新しいブランチを作成：`git checkout -b add-new-api`
3. API を適切なカテゴリーに追加（アルファベット順を保持）
4. 変更をコミット：`git commit -m "Add XXX API to Category"`
5. Fork にプッシュ：`git push origin add-new-api`
6. `master` ブランチに Pull Request を提出

> ⚠️ **注意**：PR を提出すると、リンクの有効性チェックが自動的に実行されます。すべてのリンクが正常にアクセスできることを確認してください。

詳細な貢献ガイドは [CONTRIBUTING.md](./CONTRIBUTING.md)（英語）をご覧ください。

---

## アップストリームとの同期

この Fork は定期的に元のリポジトリの更新を同期します：

```bash
# 元のリポジトリをアップストリームとして追加
git remote add upstream https://github.com/public-apis/public-apis.git

# アップストリームの更新を取得
git fetch upstream

# ローカルのマスターブランチにマージ
git checkout master
git merge upstream/master

# Fork にプッシュ
git push origin master
```

---

## 関連リンク

- 🌐 **元のリポジトリ**：[public-apis/public-apis](https://github.com/public-apis/public-apis)
- 🍴 **この Fork**：[gumi-ink/public-apis](https://github.com/gumi-ink/public-apis)
- 📝 **貢献ガイド**：[CONTRIBUTING.md](./CONTRIBUTING.md)
- 📄 **ライセンス**：[MIT License](./LICENSE)

---

## ライセンス

このプロジェクトは [MIT License](./LICENSE) の下で公開されています。

元のプロジェクトはコミュニティメンバーと [APILayer](https://apilayer.com/) チームによって管理されています。この日本語版 Fork は [gumi-ink](https://github.com/gumi-ink) によって管理されています。

---

*最終更新：2026年3月*
