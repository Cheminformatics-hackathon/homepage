---
layout: page
title: "Venue / Access"
subtitle: "会場・アクセス・宿泊情報"
description: "ケモインフォマティクス×ハッカソン合宿の会場情報・アクセス方法・宿泊案内です。"
permalink: /venue/
---

## 会場情報

| 項目 | 詳細 |
|------|------|
| **施設名** | {{ site.data.site.venue.name }} |
| **住所** | {{ site.data.site.venue.address }} |
| **アクセス** | {{ site.data.site.venue.access }} |

{% if site.data.site.venue.map_embed != "" %}
<div class="ratio ratio-16x9 my-4">
  {{ site.data.site.venue.map_embed }}
</div>
{% elsif site.data.site.venue.map_url != "" %}
<p class="my-3">
  <a href="{{ site.data.site.venue.map_url }}" target="_blank" rel="noopener" class="btn btn-outline-navy">
    <i class="bi bi-geo-alt me-1"></i> Google Mapで見る
  </a>
</p>
{% else %}
<div class="alert alert-info my-3">
  <i class="bi bi-info-circle me-1"></i> 会場の詳細は決まり次第掲載します。
</div>
{% endif %}

---

## 宿泊について

<div class="card border-0 shadow-sm my-3">
  <div class="card-body">
    <div class="row">
      <div class="col-md-6">
        <h5 class="fw-bold"><i class="bi bi-door-open me-2"></i>チェックイン / チェックアウト</h5>
        <ul>
          <li><strong>チェックイン:</strong> TBA</li>
          <li><strong>チェックアウト:</strong> TBA</li>
        </ul>
        <h5 class="fw-bold mt-3"><i class="bi bi-egg-fried me-2"></i>食事</h5>
        <ul>
          <li>朝食・昼食・夕食が含まれる予定です</li>
          <li>アレルギー等は事前にお知らせください</li>
        </ul>
      </div>
      <div class="col-md-6">
        <h5 class="fw-bold"><i class="bi bi-bag me-2"></i>アメニティ・設備</h5>
        <ul>
          <li>タオル・シャンプー等：TBA（要確認）</li>
          <li>Wi-Fi：あり（予定）</li>
          <li>電源：各部屋および作業スペースに設置</li>
        </ul>
        <h5 class="fw-bold mt-3"><i class="bi bi-backpack me-2"></i>持ち物</h5>
        <ul>
          <li>ノートPC（必須）、充電器</li>
          <li>着替え、洗面用具</li>
          <li>電源タップ（推奨）</li>
        </ul>
      </div>
    </div>
  </div>
</div>

---

## 注意事項

<div class="alert alert-secondary">
  <ul class="mb-0">
    <li>作業スペースは24時間利用可能の予定ですが、深夜帯は他の参加者への配慮をお願いします。</li>
    <li>会場のWi-Fi環境には限りがある場合があります。大容量データのダウンロードは事前に済ませてください。</li>
    <li>貴重品の管理は各自でお願いします。</li>
    <li>施設のルールに従ってご利用ください。</li>
  </ul>
</div>
