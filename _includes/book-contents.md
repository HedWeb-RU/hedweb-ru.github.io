<h3>Содержание:</h3>

<ul style="list-style-type: none">
<li><a href="{{ site.baseurl }}/hi/abstract.html">Аннотация</a></li>
<li>{% if include.open %}<details open>{% else %}<details>{% endif %}<summary>0. <a href="{{ site.baseurl }}/hi/introduction.html">Введение</a></summary><ul>{% for a in site.data.book %}{% if a.chapter == 0 %}<li><a href="{{ site.baseurl }}/hi/introduction.html#{{ a.section }}">0.{{ a.section }}</a>. <a href="{{ site.baseurl }}/hi/introduction/{{ a.id }}.html" style="color:black">{{ a.title }}</a></li>{% endif %}{% endfor %}</ul></details></li>
<li>{% if include.open %}<details open>{% else %}<details>{% endif %}<summary>1. <a href="{{ site.baseurl }}/hi/how.html">Как?</a></summary><ul>{% for a in site.data.book %}{% if a.chapter == 1 %}<li><a href="{{ site.baseurl }}/hi/how.html#{{ a.section }}">1.{{ a.section }}</a>. <a href="{{ site.baseurl }}/hi/how/{{ a.id }}.html" style="color:black">{{ a.title }}</a></li>{% endif %}{% endfor %}</ul></details></li>
<li>{% if include.open %}<details open>{% else %}<details>{% endif %}<summary>2. <a href="{{ site.baseurl }}/hi/why.html">Зачем?</a></summary><ul>{% for a in site.data.book %}{% if a.chapter == 2 %}<li>{% if a.published %}<a href="{{ site.baseurl }}/hi/why.html#{{ a.section }}">2.{{ a.section }}</a>. <a href="{{ site.baseurl }}/hi/why/{{ a.id }}.html" style="color:black">{{ a.title }}</a>{% else %}2.{{ a.section }}. {{ a.title }} <b>— скоро добавим!</b>{% endif %}</li>{% endif %}{% endfor %}</ul></details></li>
<li>3. Когда? <b>— скоро добавим!</b></li>
<li>4. Возражения <b>— скоро добавим!</b></li>
<li>5. Заключение <b>— скоро добавим!</b></li>
</ul>
