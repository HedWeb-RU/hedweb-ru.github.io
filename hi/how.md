---
layout: book
title: Гедонистический императив
subtitle: "1. Как?"
authors:
  - Дэвид Пирс
original: "https://www.hedweb.com"
original_date:
  - 1995
excerpt: "«Господь на небесах — с миром всё в порядке!» — Роберт Браунинг. 1.0. Бунт на фабрике. Чтобы сойти с гедонистической беговой дорожки, сначала мы должны избавиться от небольшого, но порочного набора механизмов обратной связи, которые генетически запрограммированы в нашем мозге и разуме."
---
<h1>1. Как?</h1>

> Господь на небесах —<br>
> С миром всё в порядке!<br>
> &nbsp;&nbsp;&nbsp;&nbsp; — Роберт Браунинг

{% for p in site.data.book %}{% if p.chapter == 1 %}
<a id="{{ p.section }}"></a>
## {{ p.chapter }}.{{ p.section }}. {{ p.title }}

{% include hi/{{ p.chapter }}/{{ p.section }}-{{ p.id }}.md %}
{% endif %}{% endfor %}

<hr>

{% include book-contents.md %}
