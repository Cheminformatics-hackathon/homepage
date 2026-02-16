---
layout: page
title: "Program"
subtitle: "日程・タイムテーブル"
description: "ケモインフォマティクス×ハッカソン合宿のプログラム・タイムテーブルをご確認いただけます。"
permalink: /program/
---

{% if site.data.program.notice %}
<div class="alert alert-warning d-flex align-items-center" role="alert">
  <i class="bi bi-exclamation-triangle-fill me-2"></i>
  <div>{{ site.data.program.notice }}</div>
</div>
{% endif %}

<!-- Day Tabs -->
<ul class="nav nav-tabs mb-4" id="programTab" role="tablist">
  {% for day in site.data.program.days %}
  <li class="nav-item" role="presentation">
    <button class="nav-link {% if forloop.first %}active{% endif %}" id="tab-{{ day.label | slugify }}" data-bs-toggle="tab" data-bs-target="#pane-{{ day.label | slugify }}" type="button" role="tab" aria-controls="pane-{{ day.label | slugify }}" aria-selected="{% if forloop.first %}true{% else %}false{% endif %}">
      <strong>{{ day.label }}</strong>
      {% if day.date != "TBA" %}<small class="text-muted ms-1">{{ day.date }}</small>{% endif %}
    </button>
  </li>
  {% endfor %}
</ul>

<!-- Tab Content -->
<div class="tab-content" id="programTabContent">
  {% for day in site.data.program.days %}
  <div class="tab-pane fade {% if forloop.first %}show active{% endif %}" id="pane-{{ day.label | slugify }}" role="tabpanel" aria-labelledby="tab-{{ day.label | slugify }}">

    <div class="table-responsive">
      <table class="table table-program">
        <thead>
          <tr>
            <th style="width: 15%;">時間</th>
            <th style="width: 45%;">内容</th>
            <th style="width: 20%;">場所</th>
            <th style="width: 20%;">担当</th>
          </tr>
        </thead>
        <tbody>
          {% for session in day.sessions %}
          <tr class="session-{{ session.type }}">
            <td class="fw-medium">{{ session.time }}</td>
            <td>{{ session.title }}</td>
            <td class="text-muted">{{ session.location }}</td>
            <td class="text-muted">{{ session.speaker }}</td>
          </tr>
          {% endfor %}
        </tbody>
      </table>
    </div>

  </div>
  {% endfor %}
</div>

---

### セッション種別

<div class="row g-2 mt-2">
  <div class="col-auto"><span class="badge" style="background:#e8a838;">基調講演</span></div>
  <div class="col-auto"><span class="badge" style="background:#28a745;">ハッカソン</span></div>
  <div class="col-auto"><span class="badge" style="background:#6f42c1;">ワークショップ</span></div>
  <div class="col-auto"><span class="badge" style="background:#0d6efd;">発表・トーク</span></div>
  <div class="col-auto"><span class="badge" style="background:#e83e8c;">交流会</span></div>
  <div class="col-auto"><span class="badge" style="background:#6c757d;">一般</span></div>
</div>
