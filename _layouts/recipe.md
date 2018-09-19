---
layout: default
---

<h1>{{ page.title }}</h1>

{% if page.ingredients %}
<b>Ingredients:</b>
<ul>
{% for ingredient in page.ingredients %}
  <li>{{ ingredient }}
{% endfor %}
</ul>
{% endif %}

{% if page.serves %}
<p><b>Serves {{ page.serves }}</b></p>
{% endif %}

{% if page.source %}
<p><b>Source:</b> <a href="{{ page.source.url | default: page.source }}">{{ page.source.name | default: page.source }}</a></p>
{% endif %}

{{ content }}
