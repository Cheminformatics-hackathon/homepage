---
layout: page
title: "Themes"
subtitle: "テーマ・プロジェクト例"
description: "ケモインフォマティクス×ハッカソン合宿で取り組めるテーマやプロジェクト例を紹介します。"
permalink: /themes/
---

ハッカソンで取り組むテーマの例を紹介します。運営が用意するテーマのほか、**自分のテーマを持ち込んでの参加も大歓迎** です。

<div class="row g-4 mt-3">
  {% for theme in site.data.themes %}
  <div class="col-md-6">
    <div class="card h-100 border-0 shadow-sm theme-card position-relative">
      <span class="theme-type-badge badge {% if theme.type == '運営テーマ' %}bg-navy{% else %}bg-accent{% endif %}">{{ theme.type }}</span>
      <div class="card-body">
        <h5 class="card-title fw-bold">{{ theme.title }}</h5>
        <p class="card-text text-muted">{{ theme.description }}</p>
        <div class="mb-2">
          {% for tag in theme.tags %}
          <span class="badge bg-light text-navy border me-1">{{ tag }}</span>
          {% endfor %}
        </div>
        <div class="d-flex justify-content-between small text-muted">
          <span><i class="bi bi-speedometer2 me-1"></i>{{ theme.difficulty }}</span>
          <span><i class="bi bi-box-arrow-up me-1"></i>{{ theme.output }}</span>
        </div>
      </div>
    </div>
  </div>
  {% endfor %}
</div>

---

## 成果物について

各チームは最終日に **成果発表** を行います。以下の形式が推奨されます。

| 形式 | 内容 |
|------|------|
| **プレゼンテーション** | 5〜10分程度のスライド発表（学会発表形式） |
| **デモ** | 動くプロトタイプやJupyter Notebookのデモンストレーション |
| **GitHubリポジトリ** | コード・データ・READMEを含むリポジトリの公開 |
| **ポスター** | （任意）研究ポスター形式でのまとめ |

> テーマの追加・変更は随時行われる可能性があります。最新情報はこのページをご確認ください。
