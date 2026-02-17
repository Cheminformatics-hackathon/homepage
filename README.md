# ケモインフォマティクス×ハッカソン合宿 公式サイト

GitHub Pages + Jekyll で公開する静的サイトです。  
トップページは「学会サイト風デザイン」をベースにしています。

## 技術スタック
- Jekyll（GitHub Pages）
- Bootstrap 5（CDN）
- カスタムCSS（`assets/css/custom.css`）

## ディレクトリ構成
```text
homepage/
├── _config.yml
├── _data/
│   ├── site.yml
│   ├── navigation.yml
│   ├── news.yml
│   ├── themes.yml
│   ├── program.yml
│   └── faq.yml
├── _includes/
│   ├── head.html
│   ├── nav.html
│   ├── footer.html
│   └── home/
│       ├── hero.html
│       ├── news_and_sidebar.html
│       └── themes.html
├── _layouts/
│   ├── default.html
│   ├── home.html
│   └── page.html
├── assets/
│   ├── css/custom.css
│   └── img/
├── index.md
├── about.md
├── program.md
├── themes.md
├── venue.md
├── registration.md
├── faq.md
├── contact.md
└── sponsors.md
```

## どこを編集すればよいか
- サイト基本情報: `_data/site.yml`
- メニュー項目: `_data/navigation.yml`
- お知らせ: `_data/news.yml`
- テーマ一覧: `_data/themes.yml`
- トップページ構造: `_includes/home/*.html`
- 全体デザイン調整: `assets/css/custom.css`

## トップページの保守ルール
- トップ構造は `_layouts/home.html` で直接書かず、`_includes/home/` に分割して管理する。
- ナビ項目は `nav.html` で直書きせず、`_data/navigation.yml` を編集する。
- 余白・文字位置・横並び挙動は `custom.css` の以下ブロックを優先して調整する。
  - `.main-nav*`
  - `.hero-*`
  - `.home-grid`
  - `.panel*`

## GitHub Pages 公開
1. GitHub リポジトリの `Settings > Pages` を開く
2. `Deploy from a branch` を選択
3. `main` / `/(root)` を指定して保存
4. `https://<username>.github.io/<repo>/` で公開

`_config.yml` の `baseurl` はリポジトリ名に合わせてください。

## ローカル確認
```bash
bundle install
bundle exec jekyll serve
```

## 注意
- 画像は `assets/img/` 配下に配置してください。
- スポンサーロゴを実画像化する場合は、`_includes/home/news_and_sidebar.html` の協賛リスト部分を差し替えてください。
