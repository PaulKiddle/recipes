---
layout: default
---

{% if page.ingredients %}
<b>Ingredients:</b>
<ul>
{% for ingredient in page.ingredients %}
  <li>{{ ingredient }}
{% endfor %}
</ul>
{% endif %}

{{ content }}
