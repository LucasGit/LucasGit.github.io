# HTML 文件列表

<ul>
{% for page in site.pages %}
  {% if page.path contains ".html" %}
    <li><a href="{{ page.url }}">{{ page.path }}</a></li>
  {% endif %}
{% endfor %}
</ul>

