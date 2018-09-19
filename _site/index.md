<h1>{{ site.name }}</h1>

<ul>
{% for post in site.recipes %}
  <li><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
{% endfor %}
</ul>
