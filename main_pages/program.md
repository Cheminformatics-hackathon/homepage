---
layout: page
title: "Event"
subtitle: "開催案内・プログラム"
description: "ケモインフォマティクス×ハッカソン合宿のプログラム・タイムテーブルをご確認いただけます。"
permalink: /program/
body_class: event-page
---

<section class="event-ribbon-block">
  <h2 class="event-ribbon-title mb-0">イベント開催案内</h2>
</section>

<section class="event-announcement-block">
  <div class="event-announcement-head">
    <h3>ケモインフォマティクス×ハッカソン合宿 開催のお知らせ</h3>
    <p class="event-updated mb-0">更新日: {{ site.time | date: "%Y/%m/%d" }}</p>
  </div>

  <div class="event-announcement-body">
    <p class="mb-2"><strong>【会期】</strong> {{ site.data.site.date.display }}</p>
    <p class="mb-2"><strong>【会場】</strong> {{ site.data.site.venue.name }}</p>
    {% if site.data.site.venue.address and site.data.site.venue.address != "TBA" %}
    <p class="mb-2 ps-4">{{ site.data.site.venue.address }}</p>
    {% endif %}
    <p class="mb-0">詳細は、決まり次第このページで更新します。</p>
  </div>
</section>

<section class="event-records-block">
  <h3 class="event-section-title">イベント記録</h3>
  <div class="table-responsive">
    <table class="table event-records-table mb-0">
      <thead>
        <tr>
          <th style="width: 14%;">回</th>
          <th style="width: 26%;">会場</th>
          <th style="width: 22%;">会期</th>
          <th style="width: 18%;">備考</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <th><a class="event-record-link" href="{{ '/program/info_1/' | relative_url }}">第1回</a></th>
          <td>横浜市上郷・森の家</td>
          <td>2025/8/28 ~ 2025/8/29</td>
          <td><a class="event-record-link" href="{{ '/program/report_1/' | relative_url }}">開催報告</a></td>
        </tr>
        <tr>
          <th><a class="event-record-link" href="{{ '/program/info_2/' | relative_url }}">第2回</a></th>
          <td>{{ site.data.site.venue.name }}</td>
          <td>{{ site.data.site.date.display }}</td>
          <td>準備中</td>
        </tr>
      </tbody>
    </table>
  </div>
</section>
