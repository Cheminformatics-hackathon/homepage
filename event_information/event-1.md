---
layout: page
title: "Event"
subtitle: "第1回 イベント詳細"
description: "第1回ケモインフォマティクス×ハッカソン合宿の開催概要・詳細ページ"
permalink: /program/info_1/
body_class: event-page
---

<section class="event-ribbon-block">
  <h2 class="event-ribbon-title mb-0">第1回 イベント詳細</h2>
</section>

<section class="event-announcement-block">
  <div class="event-announcement-head">
    <h3>第1回 ケモインフォマティクス×ハッカソン合宿</h3>
    <p class="event-updated mb-0">更新日: {{ site.time | date: "%Y/%m/%d" }}</p>
  </div>

  <div class="event-announcement-body">
    <p class="mb-2"><strong>【年度】</strong> 2026</p>
    <p class="mb-2"><strong>【会期】</strong> {{ site.data.site.date.display }}</p>
    <p class="mb-2"><strong>【会場】</strong> {{ site.data.site.venue.name }}</p>
    {% if site.data.site.venue.address and site.data.site.venue.address != "TBA" %}
    <p class="mb-2 ps-4">{{ site.data.site.venue.address }}</p>
    {% endif %}
    <p class="mb-0">本ページに第1回の詳細情報（募集要項、当日案内、発表内容など）を掲載していきます。</p>
  </div>
</section>

<section class="event-records-block">
  <h3 class="event-section-title">掲載予定情報</h3>
  <ul class="mb-0">
    <li>開催概要・参加対象</li>
    <li>タイムテーブル</li>
    <li>会場案内・アクセス</li>
    <li>成果発表・記録</li>
  </ul>
</section>

<div class="text-center mt-3">
  <a href="{{ '/program/' | relative_url }}" class="btn btn-outline-navy btn-sm">
    <i class="bi bi-arrow-left me-1"></i>Event一覧に戻る
  </a>
</div>
