---
layout: page
title: "Registration"
subtitle: "参加登録"
description: "ケモインフォマティクス×ハッカソン合宿への参加登録方法・参加費・締切などの情報です。"
permalink: /registration/
---

## 参加登録

{% if site.data.site.registration.status == "受付中" %}
<span class="status-badge status-open mb-3 d-inline-block"><i class="bi bi-check-circle me-1"></i>現在受付中</span>
{% elsif site.data.site.registration.status == "締切" %}
<span class="status-badge status-closed mb-3 d-inline-block"><i class="bi bi-x-circle me-1"></i>受付終了</span>
{% else %}
<span class="status-badge status-preparing mb-3 d-inline-block"><i class="bi bi-clock me-1"></i>準備中</span>
{% endif %}

<div class="card border-0 shadow-sm my-4">
  <div class="card-body">
    <table class="table table-borderless mb-0">
      <tbody>
        <tr>
          <th style="width:30%;" class="text-navy"><i class="bi bi-people me-2"></i>定員</th>
          <td>{{ site.data.site.registration.capacity }}</td>
        </tr>
        <tr>
          <th class="text-navy"><i class="bi bi-cash me-2"></i>参加費</th>
          <td>{{ site.data.site.registration.fee }}</td>
        </tr>
        <tr>
          <th class="text-navy"><i class="bi bi-calendar-check me-2"></i>申込締切</th>
          <td>{{ site.data.site.registration.deadline }}</td>
        </tr>
        <tr>
          <th class="text-navy"><i class="bi bi-credit-card me-2"></i>支払い方法</th>
          <td>TBA</td>
        </tr>
      </tbody>
    </table>
  </div>
</div>

{% if site.data.site.registration.status == "受付中" %}
<div class="text-center my-4">
  <a href="{{ site.data.site.registration.form_url }}" class="btn btn-accent btn-lg" target="_blank" rel="noopener">
    <i class="bi bi-pencil-square me-2"></i>参加登録フォームへ
  </a>
</div>
{% endif %}

---

## 推奨する事前準備

参加をより充実させるために、以下の準備をお勧めします（必須ではありません）。

<div class="row g-3 my-3">
  <div class="col-md-6">
    <div class="card h-100 border-0 shadow-sm p-3">
      <h6 class="fw-bold"><i class="bi bi-terminal me-2 text-navy"></i>Python環境</h6>
      <p class="text-muted small mb-0">Anaconda / Miniconda をインストールし、Python 3.9以上の環境を準備してください。</p>
    </div>
  </div>
  <div class="col-md-6">
    <div class="card h-100 border-0 shadow-sm p-3">
      <h6 class="fw-bold"><i class="bi bi-github me-2 text-navy"></i>GitHubアカウント</h6>
      <p class="text-muted small mb-0">アカウントを作成し、基本的なGit操作（clone, commit, push）に慣れておくと便利です。</p>
    </div>
  </div>
  <div class="col-md-6">
    <div class="card h-100 border-0 shadow-sm p-3">
      <h6 class="fw-bold"><i class="bi bi-journal-code me-2 text-navy"></i>RDKit（任意）</h6>
      <p class="text-muted small mb-0"><code>conda install -c conda-forge rdkit</code> でインストールできます。当日もセットアップのサポートを行います。</p>
    </div>
  </div>
  <div class="col-md-6">
    <div class="card h-100 border-0 shadow-sm p-3">
      <h6 class="fw-bold"><i class="bi bi-book me-2 text-navy"></i>基礎知識（任意）</h6>
      <p class="text-muted small mb-0">ケモインフォマティクスの入門資料に目を通しておくとスムーズです。</p>
    </div>
  </div>
</div>

---

## キャンセルポリシー

- 申込後のキャンセルは、所定の期限までにご連絡ください。
- 期限を過ぎてのキャンセルは、キャンセル料が発生する場合があります。
- 詳細は参加登録時にお知らせします。

---

<div class="text-center mt-4">
  <p class="text-muted">ご不明な点は <a href="{{ '/contact' | relative_url }}">お問い合わせ</a> からご連絡ください。</p>
</div>
