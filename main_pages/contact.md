---
layout: page
title: "Contact"
subtitle: "お問い合わせ"
description: "ケモインフォマティクス×ハッカソン合宿へのお問い合わせ方法です。"
permalink: /contact/
---

## お問い合わせ方法

ご質問・ご相談はお気軽に以下の方法でお問い合わせください。

<div class="row g-4 my-4">
  <div class="col-md-6">
    <div class="card h-100 border-0 shadow-sm text-center p-4">
      <div class="card-body">
        <h3 class="fw-bold">メール</h3>
        {% if site.data.site.links.email != "TBA" and site.data.site.links.email != "" %}
        <p class="mb-0"><a href="mailto:{{ site.data.site.links.email }}">{{ site.data.site.links.email }}</a></p>
        {% else %}
        <p class="mb-0 text-muted">TBA（準備中）</p>
        {% endif %}
      </div>
    </div>
  </div>
  <div class="col-md-6">
    <div class="card h-100 border-0 shadow-sm text-center p-4">
      <div class="card-body">
        <h3 class="fw-bold">五東研究室 ホームページ</h3>
        {% if site.data.site.links.github != "" %}
        <p class="mb-0"><a href="{{ site.data.site.links.homepage }}" target="_blank" rel="noopener">{{ site.data.site.links.homepage }}</a></p>
        {% else %}
        <p class="mb-0 text-muted">TBA</p>
        {% endif %}
      </div>
    </div>
  </div>
  <div class="col-md-6">
    <div class="card h-100 border-0 shadow-sm text-center p-4">
      <div class="card-body">
        <h3 class="fw-bold">GitHub</h>
        {% if site.data.site.links.github != "" %}
        <p class="mb-0"><a href="{{ site.data.site.links.github }}" target="_blank" rel="noopener">GitHub Organization</a></p>
        {% else %}
        <p class="mb-0 text-muted">TBA</p>
        {% endif %}
      </div>
    </div>
  </div>
</div>

{% if site.data.site.links.twitter != "" %}
<div class="row g-4 mb-4">
  <div class="col-md-6 mx-auto">
    <div class="card border-0 shadow-sm text-center p-4">
      <div class="card-body">
        <i class="bi bi-twitter-x fs-1 text-navy d-block mb-3"></i>
        <h5 class="fw-bold">X (Twitter)</h5>
        <p class="mb-0"><a href="{{ site.data.site.links.twitter }}" target="_blank" rel="noopener">@アカウント名</a></p>
      </div>
    </div>
  </div>
</div>
{% endif %}

---

## 運営

<table class="table">
  <tbody>
    <tr>
      <th class="text-navy" style="width:30%;">運営団体</th>
      <td>{{ site.data.site.organizer.name }}</td>
    </tr>
    <tr>
      <th class="text-navy">連絡先</th>
      <td>{{ site.data.site.organizer.contact }}</td>
    </tr>
  </tbody>
</table>

---

<div class="alert alert-info">
  <i class="bi bi-clock me-2"></i>
  お問い合わせへの返信は <strong>数日以内</strong> を目安にお返事いたします。お急ぎの場合はその旨をお伝えください。
</div>
