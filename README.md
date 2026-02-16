# ケモインフォマティクス×ハッカソン合宿 公式サイト

> GitHub Pages + Jekyll で運用する学会風イベントサイト

## 🏗️ 技術構成

- **静的サイトジェネレータ**: Jekyll（GitHub Pages標準）
- **CSSフレームワーク**: Bootstrap 5（CDN）
- **フォント**: Noto Sans JP / Inter（Google Fonts）

---

## 📁 ディレクトリ構成

```
homepage/
├── _config.yml           # Jekyll設定（baseurl等）
├── _layouts/             # ページテンプレート
│   ├── default.html      # 全ページ共通の外枠
│   ├── home.html         # トップページ専用
│   └── page.html         # 一般ページ用
├── _includes/            # 共通パーツ
│   ├── head.html         # <head>タグ（CSS, Meta, OGP）
│   ├── nav.html          # ナビゲーションバー
│   ├── footer.html       # フッター
│   ├── hero.html         # トップのヒーロー領域
│   └── news.html         # お知らせ一覧
├── _data/                # ★ 運営が主に編集するデータ
│   ├── site.yml          # イベント基本情報
│   ├── program.yml       # タイムテーブル
│   ├── faq.yml           # FAQ
│   ├── news.yml          # お知らせ
│   └── themes.yml        # テーマ例
├── assets/
│   ├── css/custom.css    # カスタムスタイル
│   └── img/              # 画像格納
├── index.md              # トップページ
├── about.md              # 概要
├── program.md            # プログラム
├── themes.md             # テーマ
├── venue.md              # 会場・アクセス
├── registration.md       # 参加登録
├── faq.md                # FAQ
├── contact.md            # お問い合わせ
├── code-of-conduct.md    # 行動規範
└── sponsors.md           # 協賛
```

---

## 🔄 コンテンツの更新方法

### 基本情報（日程・場所・参加費など）を変更したい

→ **`_data/site.yml`** を編集してください。ここの値は全ページに自動反映されます。

```yaml
# 例: 日程を更新
date:
  start: "2026-08-01"
  end: "2026-08-03"
  display: "2026年8月1日（土）〜 8月3日（月）"
```

### プログラム（タイムテーブル）を変更したい

→ **`_data/program.yml`** を編集してください。

### FAQを追加・編集したい

→ **`_data/faq.yml`** を編集してください。カテゴリとアイテムを追加するだけでOKです。

### お知らせを追加したい

→ **`_data/news.yml`** の先頭に新しいエントリを追加してください。

```yaml
- date: "2026-04-01"
  title: "参加登録を開始しました"
  content: "詳細は Registration ページをご覧ください。"
  badge: "NEW"
```

### テーマを追加・編集したい

→ **`_data/themes.yml`** を編集してください。

### 画像を追加したい

→ **`assets/img/`** フォルダに配置してください。

- スポンサーロゴ: `assets/img/sponsors/`
- OGP画像: `assets/img/ogp.png`
- favicon: `assets/img/favicon.ico`

---

## 🚀 GitHub Pages 公開手順

### 初回設定

1. GitHubリポジトリの **Settings** > **Pages** を開く
2. **Source** で `Deploy from a branch` を選択
3. **Branch** で `main` / `/ (root)` を選択して **Save**
4. 数分後に `https://<username>.github.io/homepage/` で公開される

### `baseurl` の変更

リポジトリ名を変更した場合は `_config.yml` の `baseurl` を合わせて変更してください:

```yaml
baseurl: "/your-repo-name"
```

---

## 💻 ローカルで確認する（任意）

```bash
# Ruby / Bundler が必要
gem install bundler jekyll

# 依存関係のインストール
bundle install

# ローカルサーバ起動
bundle exec jekyll serve

# http://localhost:4000/homepage/ で確認
```

### Gemfile（必要に応じて作成）

```ruby
source "https://rubygems.org"
gem "jekyll", "~> 4.3"
gem "jekyll-seo-tag"
```

---

## 📝 運用メモ

- **TBA表示**: `_data/site.yml` の値を `"TBA"` にすると全ページでTBA表示になります
- **参加登録ステータス**: `_data/site.yml` の `registration.status` を `"受付中"` / `"準備中"` / `"締切"` で切り替え
- **ページの追加**: 新しい `.md` ファイルをルートに作成し、Front Matter で `layout: page` / `permalink` を指定
- **ナビゲーション**: メニュー項目を追加する場合は `_includes/nav.html` を編集

---

## 📄 ライセンス

MIT License