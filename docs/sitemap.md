---
---

{% for cat in site.category-list %}
### {{ cat }}
<ul>
  {% for page in site.pages %}
    {% if page.dnd == true %}
      {% for pc in page.categories %}
        {% if pc == cat %}
          <li><a href="{{site.baseurl}}{{ page.url }}">{{ page.title }}</a></li>
        {% endif %} 
      {% endfor %}
    {% endif %}
  {% endfor %}
</ul>
{% endfor %} 