---
layout: page
title: "FAQ"
subtitle: "よくある質問"
description: "ケモインフォマティクス×ハッカソン合宿に関するよくある質問と回答です。"
permalink: /faq/
body_class: faq-page
---

{% for category in site.data.faq.categories %}
<section class="faq-category-block">
  <h2 class="faq-category-title">
    {{ category.name }}
  </h2>

  {% for item in category.items %}
  <div class="faq-item mb-4">
    <h3 class="faq-question fw-bold">
      {{ item.question }}
    </h3>
    <div class="faq-answer text-muted mt-2">
      {{ item.answer }}
    </div>
  </div>
  {% endfor %}
</section>
{% endfor %}


<div class="faq-footer-cta text-center">
  <p class="mb-0">その他のご質問は <a href="{{ '/contact' | relative_url }}" class="btn btn-outline-navy btn-sm"><i class="bi bi-envelope me-1"></i>お問い合わせ</a> からお気軽にどうぞ。</p>
</div>
