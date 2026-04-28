# ケモインフォマティクス×ハッカソン合宿 公式サイト（Jekyll）

GitHub Pages + Jekyll で公開する静的サイトです。  
現在のナビゲーションは `Home / About / Event / FAQ / Contact` の構成です。

## 公開URL

https://cheminformatics-hackathon.github.io/homepage/

## ローカル確認
```bash
bundle install
bundle exec jekyll serve
```

補足:
- `bundler` のバージョン不一致が出る場合は、`Gemfile.lock` に合わせて Bundler を入れてください（例: `gem install bundler:4.0.6`）。

## 現在のページ構成（どこを編集するか）

### 1) サイト全体の基本情報
- `_data/site.yml`
- イベント名、英語名、キャッチコピー、開催情報、会場情報、連絡先など
- Home / Event / Footer など複数ページに反映されます

### 2) ナビゲーション（メニュー）
- `_data/navigation.yml`
- ナビの順番・表示名・リンク先を編集
- 現在 `Event` は `/program` にリンクしています（ページファイルは `program.md`）

### 3) Home（トップページ）
- `index.md`
  - 追加文面を入れたい場合（通常は空でもOK）
- `_layouts/home.html`
  - Home にどのブロックを表示するか（現在は Hero + News）
- `_includes/home/hero.html`
  - 上部ヒーロー（タイトル、日程、会場、対象表示）
- `_includes/home/news_and_sidebar.html`
  - NEWS、お知らせ、イベントカード、協賛欄
- `_data/news.yml`
  - NEWS一覧の内容

### 4) About ページ
- `about.md`
- 現在は「本イベントについて」のブロックのみ表示
- About の本文を変えたいときはこのファイルを編集

### 5) Event ページ（イベント一覧/記録）
- `program.md`
- ナビの `Event` から開くページ（URL: `/program/`）
- 「イベント開催案内」と「イベント記録」表の内容を編集
- 記録表の各回リンクもここで設定

### 6) Event の各回詳細ページ
- `events/` フォルダ
- 例: `events/event-1.md`（現在の第1回詳細ページ）
- URL は各ファイルの `permalink` で管理（例: `/program/1/`）
- 第2回以降を追加する場合:
  - `events/event-2.md` を作成
  - `permalink: /program/2/` を設定
  - `program.md` のイベント記録表にリンクを追加

### 7) FAQ ページ
- `faq.md`
  - FAQページの構造・説明文・CTA
- `_data/faq.yml`
  - 質問と回答のデータ本体（カテゴリ含む）

### 8) Contact ページ
- `contact.md`
- お問い合わせ方法や案内文の編集

### 9) Sponsors ページ
- `sponsors.md`
- 協賛募集・スポンサー情報のページ
- Home のサイドバーからリンクされています

## デザイン調整（見た目を変える場所）

### 最優先（ほとんどここ）
- `assets/css/custom.css`
- 余白、文字位置、色、ホバー、各ページのパネルデザインを調整

よく触る箇所の例:
- ナビ: `.main-nav*`, `.navbar-brand`, `.main-nav-list`
- Homeヒーロー: `.hero-*`
- 共通ページ枠: `.page-*`
- About: `.about-*`
- FAQ: `.faq-*`
- Event: `.event-*`
- フッター: `.site-footer`, `.footer-*`

## レイアウト / 共通部品（構造を変える場所）
- `_layouts/default.html`
  - 全ページ共通の骨組み（`<head>`, ナビ, フッター, `<main>`）
- `_layouts/page.html`
  - About / Event / FAQ / Contact / Sponsors など共通ページレイアウト
- `_includes/nav.html`
  - ヘッダー / ナビのHTML本体
- `_includes/footer.html`
  - フッターのHTML本体
- `_includes/head.html`
  - メタタグ、CSS/JS読み込み

## Event詳細ページの運用ルール（推奨）
- 各回の詳細ページは `events/` フォルダに集約する
- 命名規則: `events/event-<回数>.md`
- URL規則: `permalink: /program/<回数>/`
- 一覧からの導線は `program.md` の「イベント記録」表で管理する

## 触らない方がよい場所（自動生成）
- `_site/`
- Jekyll の生成結果です。通常は直接編集しません。
- 見た目を変えたい場合は、必ず元ファイル（`.md`, `_includes`, `_layouts`, `assets/css/custom.css`, `_data/*.yml`）を編集してください。

## 今回削除した未使用ファイル（現状構成では未参照）
- `themes.md`
- `venue.md`
- `registration.md`
- `code-of-conduct.md`
- `_data/themes.yml`
- `_data/program.yml`
- `_includes/home/themes.html`

必要になったら `git` から復元できます。
