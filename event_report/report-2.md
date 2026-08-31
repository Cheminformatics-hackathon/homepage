---
layout: page
title: "Event"
subtitle: "第2回 開催報告"
description: "第2回ケモインフォマティクス×ハッカソン合宿の開催報告ページ"
permalink: /program/report_2/
body_class: event-page
---

<section class="event-ribbon-block">
  <h2 class="event-ribbon-title mb-0">第2回 開催報告</h2>
</section>

<section class="event-announcement-block">
  <div class="event-announcement-head">
    <h3>第2回 ケモインフォマティクス×ハッカソン合宿</h3>
    <p class="event-updated mb-0">更新日: {{ site.time | date: "%Y/%m/%d" }}</p>
  </div>

  <div class="event-announcement-body">
    <p class="mb-2"><strong>【会期】</strong> 2026/8/26 ~ 2025/8/27</p>
    <p class="mb-2"><strong>【会場】</strong> 横浜市上郷・森の家</p>
    {% if site.data.site.venue.address and site.data.site.venue.address != "TBA" %}
    <p class="mb-2 ps-4">{{ site.data.site.venue.address }}</p>
    {% endif %}
  </div>
</section>

<p style="text-align:center;">
  <img src="{{ 'assets/img/report-2/バーナー改.png' | relative_url }}" alt="イベントの様子" style="max-width: 1040px; width: 100%; height: auto;">
</p>

<section class="about-block" markdown="1">

# はじめに
近年、多くの分野の研究にAIやデータサイエンスが浸透し始め、それは化学も例外ではありません。ケモインフォマティクスは、その代表例であり分子の設計や物性予測、創薬支援などを行う学問です。日々注目度が上がっているケモインフォマティクスですが、実践的に学べる機会が少ないことが課題でした。本イベントではハッカソンを通じて実践的にケモインフォマティクスを学ぶプログラムを実施しました。学部生から博士学生、普段ウェットな実験しか行わない学生から情報工学専攻の学生まで様々なバックグラウンドを持つ方に参加していただきました。異なる専門性や視点を持つ方同士でのハッカソンなどを通じた交流は、分野横断的な発想や工夫の重要性を実感していただいたと確信しています。そんな本イベントの開催報告を簡単ながら掲載いたします。

# ハッカソンのテーマ
今回のハッカソンのテーマは、「化合物の構造情報と化合物の説明文を正しく結びつける」タスクでした。化合物の説明文は、全く化学が分からない方でも、その化合物についてある程度情報を得ることができるため重要です。化合物の説明文を生成できることがベストではありますが、マシンスペック的な制限や時間的な制限があるため、今回は生成の手前の段階である、化合物と説明文を正しく結びつけるというタスクになりました。詳しくは下の資料をご覧ください。

# 1日目
### ショートプレゼン
合宿の始めには、参加者みなさんの専門領域をできるだけみんなで共有できるように、参加任意のショートプレゼンを行いました。化学がバックグラウンドの方が多かったですが、その中でも物理化学や分析化学、生化学や計算化学など、皆さん様々な分野の研究をされていて、さらにはLLM(大規模言語モデル)を用いた情報工学の研究をされている方もおり、普段とは異なる分野の発表を聞けるよい機会になりました。またこのショートプレゼンとそのあとの班ごとのアイスブレイクで皆さんの緊張がほぐれ、よい雰囲気でハッカソンを始められました。

<p style="text-align:center;">
  <img src="{{ 'assets/img/report-2/Day1_ショートプレゼン.png' | relative_url }}" alt="イベントの様子" style="max-width: 1040px; width: 100%; height: auto;">
</p>

[ショートプレゼンプログラム](https://drive.google.com/file/d/1LK0fmSGwJNtx2jlA3SlsburgAI5zdUPk/view?usp=drive_link)

### ハッカソン
自然言語処理に触れたことのない参加者の方も多く、テーマを渡されたときは、そのテーマを理解するのに一苦労している印象を受けました。ただチームの仲間同士でテーマを噛み砕き、アプローチするべき部分をまとめ、みんなで分担しながらテーマに向き合っていました。

<p style="text-align:center;">
  <img src="{{ 'assets/img/report-2/Day1_ハッカソン1.png' | relative_url }}" alt="イベントの様子" style="max-width: 1040px; width: 100%; height: auto;">
</p>

<p style="text-align:center;">
  <img src="{{ 'assets/img/report-2/Day1_ハッカソン2.png' | relative_url }}" alt="イベントの様子" style="max-width: 1040px; width: 100%; height: auto;">
</p>

### 夕食 (BBQ)
夕食は屋外でバーベキューをしました。なかなかここまでの時間は班のメンバー以外とかかわる機会がなかったので、他の班の人との交流が多くみられました。また今回のハッカソンの話だけでなく、普段の研究の話やバイトの話、将来の話など様々な話題で盛り上がり参加者間の中がより一層深まりました。

<p style="text-align:center;">
  <img src="{{ 'assets/img/report-2/Day1_BBQ1.png' | relative_url }}" alt="イベントの様子" style="max-width: 1040px; width: 100%; height: auto;">
</p>

<p style="text-align:center;">
  <img src="{{ 'assets/img/report-2/Day1_BBQ2.png' | relative_url }}" alt="イベントの様子" style="max-width: 1040px; width: 100%; height: auto;">
</p>

<p style="text-align:center;">
  <img src="{{ 'assets/img/report-2/Day1_BBQ3.png' | relative_url }}" alt="イベントの様子" style="max-width: 1040px; width: 100%; height: auto;">
</p>

### レクリエーション
夕食後はレクリエーションを実施しました。参加者全員で「ito」というボードゲームを実施しました。数字を言葉で表現しながら価値観を共有するこのゲームでより皆さんのことを知る機会になったと思っています。またポイントをつけて班ごとに競うことでよい緊張感の中、わいわい楽しむことができました。優勝した班にはお菓子のプレゼントがありました。

# 2日目
### ハッカソン
二日目のハッカソンは、初日の成果をブラッシュアップしつつ、成果発表会に向けた準備を各班行っていました。初日はテーマの理解から始まったものが、だんだん形になって成果が出始めたことで、参加者の皆さんの二日間の取り組んできた姿勢やアプローチの素晴らしさが垣間見えました。

<p style="text-align:center;">
  <img src="{{ 'assets/img/report-2/Day2_ハッカソン1.png' | relative_url }}" alt="イベントの様子" style="max-width: 1040px; width: 100%; height: auto;">
</p>

<p style="text-align:center;">
  <img src="{{ 'assets/img/report-2/Day2_ハッカソン2.png' | relative_url }}" alt="イベントの様子" style="max-width: 1040px; width: 100%; height: auto;">
</p>

<p style="text-align:center;">
  <img src="{{ 'assets/img/report-2/Day2_ハッカソン3.png' | relative_url }}" alt="イベントの様子" style="max-width: 1040px; width: 100%; height: auto;">
</p>

### 成果報告会
本合宿最後の企画としてハッカソンの成果報告会を行いました。各班がどんな方針を立てて、どんなアプローチでタスクに対して挑んだか、挑んだ結果うまくいった点といかなかった点、うまくいった理由やいかなかった考察などを発表してもらいました。各班の班員の専門性を存分に生かしたアプローチを各班取っており、それぞれの独自性を感じることができました。参加者の方の新たな気づきの機会になったと同時に、視野の広さの重要性を実感する機会になりました。最後には各班に作ってもらった機械学習モデルの性能と、成果報告会の発表を参加者皆さん自身で評価していただくことで最優秀チームを選出しました。最優秀チームの方には賞状と副賞を贈呈しました。

<p style="text-align:center;">
  <img src="{{ 'assets/img/report-2/Day2_成果報告会1.png' | relative_url }}" alt="イベントの様子" style="max-width: 1040px; width: 100%; height: auto;">
</p>

<p style="text-align:center;">
  <img src="{{ 'assets/img/report-2/Day2_成果報告会2.png' | relative_url }}" alt="イベントの様子" style="max-width: 1040px; width: 100%; height: auto;">
</p>

<p style="text-align:center;">
  <img src="{{ 'assets/img/report-2/Day2_成果報告会3.png' | relative_url }}" alt="イベントの様子" style="max-width: 1040px; width: 100%; height: auto;">
</p>

# 参加者アンケートの結果
参加していただいたみなさんにアンケートを実施しました。参加者の方には満足度の高いイベントになりました。いただいたご意見は次回の運営に反映できるよう尽力いたします。

### アンケート結果
<p style="text-align:center;">
  <img src="{{ 'assets/img/report-2/準備_満足度.png' | relative_url }}" alt="イベントの様子" style="max-width: 1040px; width: 100%; height: auto;">
</p>

<p style="text-align:center;">
  <img src="{{ 'assets/img/report-2/当日_満足度.png' | relative_url }}" alt="イベントの様子" style="max-width: 1040px; width: 100%; height: auto;">
</p>

<p style="text-align:center;">
  <img src="{{ 'assets/img/report-2/合宿_トータル満足度.png' | relative_url }}" alt="イベントの様子" style="max-width: 1040px; width: 100%; height: auto;">
</p>

### 頂いた感想、ご意見の一部

- 参加者のレベルがある程度均一になるように分野を絞る、課題情報の提示についてアプローチの誘導等あればいいのかなと思う
- とても楽しかったです！
- もっと機械学習について学んでいればもっと主体的にできたし、自分ももっと面白かったと思います。知識をつけた状態でまたやってみたいです。
- 様々な分野の方と交流できたので勉強になりました。とても楽しかったです。
- 短時間で沢山の試行錯誤を行なっており，プロジェクトマネジメントの観点からも多くの刺激を受けることができました。今後のハッカソンも大変楽しみにしております！
- 同年代の研究仲間と繋がる機会となり、ここでの縁が新しい技術創出のきっかけを作る可能性もあるのではないかとワクワクしました。

# まとめ
第二回ケモインフォマティクス×ハッカソン合宿 in 横浜は、参加者皆さんの協力もあり、無事全日程を終えることができました。ありがとうございます。専門性や学年の異なる初対面の方とチームを組んで課題に取り組むという経験はなかなかできないものだと思いますし、それを提供できたことは誇りに思っております。また参加者の皆さんにも、このような経験を通して、専門性が違う方の視点やアプローチの重要性、自分の専門性の活かし方を実感していただけたと確信しております。近年の科学では分野の境界の曖昧化や融合が進んでいます。専門性の異なる方と協力して何かを行うというものはこれからの研究のあるべき姿度と思っておりますし、その疑似体験、第一歩として本合宿が役に立てればいいなと思い企画、運営を行いました。来年度以降も規模を大きくしつつ実施する予定です。様々なバックグラウンドを持つ方が多く参加していただけるように精進いたしますので、この記事を読んでいただいている皆さんの来年度以降の参加を楽しみにしております。また協力していただける企業様や研究室の方も募集しております。今回参加された皆さんも来年度以降もお待ちしておりますし、学会などで再びお会いできる機会があればいいなと思っております。

最後に本合宿に関わっていただいたすべての方に感謝申し上げます。来年度以降もぜひよろしくお願いいたします。

<p style="text-align:center;">
  <img src="{{ 'assets/img/report-2/Day2_集合写真.png' | relative_url }}" alt="イベントの様子" style="max-width: 1040px; width: 100%; height: auto;">
</p>

文責：第二回ケモインフォマティクス×ハッカソン合宿 in 横浜 運営代表 加藤琉久

# 次回予告
### テーマについて
第三回の合宿は、2027年8月下旬の開催を予定しております。続報をお待ちください。ハッカソンのテーマとしては「電子状態インフォマティクス」を予定しております。電子状態から、機械学習を用いて、分子の性質を解析する課題を検討しています。講師は坂口大門先生が担当いたします。坂口先生については下のサイトや論文をご覧ください。

<p style="text-align:center;">
  <img src="{{ 'assets/img/report-2/次回予告.png' | relative_url }}" alt="イベントの様子" style="max-width: 1040px; width: 100%; height: auto;">
</p>

[坂口先生のHP](https://saka-d.github.io/homepage/index.html)

[関連論文](https://doi.org/10.26434/chemrxiv.15002906/v2)

### 情報発信
今回と同様、各種SNSでも発信予定です。ぜひ定期的にチェックしてください！！

[X(旧Twitter)](https://x.com/chemoinfo_camp?s=11&t=keykxFqubZza7Mf35TYLzw)

[Instagram](https://www.instagram.com/chemoinfomatics_camp?igsi=aml3dXpxaGhyaGJi&utm_source=qr)