<!DOCTYPE html>
<html lang="ru">

{% for t in site.data.book %}{% if t.id == page.id %}{% assign p = t %}{% break %}{% endif %}{% endfor %}
{% assign pt=p.chapter | append: "." | append: p.section | append: ". " | append: p.title %}
{% assign pt1="Гедонистический императив. " | append: pt | append: " | Дэвид Пирс" %}
{% include head.html title=pt1 nopicture=true %}

<body>

{% include book-head.html %}

<div class="container content">

<div class="content">

{% if p.chapter == 0 %}{% assign chapter = "0. Введение" %}{% elsif p.chapter == 1 %}{% assign chapter = "1. Как?" %}{% elsif p.chapter == 2 %}{% assign chapter = "2. Зачем?" %}{% elsif p.chapter == 3 %}{% assign chapter = "3. Когда?" %}{% elsif p.chapter == 4 %}{% assign chapter = "4. Возражения" %}{% elsif p.chapter == 5 %}{% assign chapter = "5. Заключение" %}{% endif %}
<h3 style="margin: 0; padding: 0">{{ chapter }}</h3>
<h2>{{ pt }}</h2>

<div class="content">

{% include hi/{{ p.chapter }}/{{ p.section }}-{{ p.id }}.md %}

</div>

{% include book-contents.md %}

</div>

<hr style="margin: 8px; padding: 8px">

<a href="/index.html">► на главную</a>

</div>

</body>

</html>
