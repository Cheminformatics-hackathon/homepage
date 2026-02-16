---
layout: page
title: "FAQ"
subtitle: "よくある質問"
description: "ケモインフォマティクス×ハッカソン合宿に関するよくある質問と回答です。"
permalink: /faq/
---

以下は参加をご検討中の方からよくいただく質問です。ここに載っていない質問は [お問い合わせ]({{ '/contact' | relative_url }}) からお気軽にどうぞ。

{% for category in site.data.faq.categories %}
<h3 class="mt-5 mb-3"><i class="bi bi-folder2-open me-2"></i>{{ category.name }}</h3>

<div class="accordion mb-4" id="faq-{{ category.id }}">
  {% for item in category.items %}
  <div class="accordion-item">
    <h2 class="accordion-header" id="heading-{{ category.id }}-{{ forloop.index }}">
      <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapse-{{ category.id }}-{{ forloop.index }}" aria-expanded="false" aria-controls="collapse-{{ category.id }}-{{ forloop.index }}">
        {{ item.question }}
      </button>
    </h2>
    <div id="collapse-{{ category.id }}-{{ forloop.index }}" class="accordion-collapse collapse" aria-labelledby="heading-{{ category.id }}-{{ forloop.index }}" data-bs-parent="#faq-{{ category.id }}">
      <div class="accordion-body text-muted">
        {{ item.answer }}
      </div>
    </div>
  </div>
  {% endfor %}
</div>
{% endfor %}

---

<div class="text-center mt-4">
  <p>その他のご質問は <a href="{{ '/contact' | relative_url }}" class="btn btn-outline-navy btn-sm"><i class="bi bi-envelope me-1"></i>お問い合わせ</a> からお気軽にどうぞ。</p>
</div>
