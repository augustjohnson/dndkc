---
---
### Version 1.4

{% for category in site.pages[categories] %}
#{{category}}
{% for page in site.pages %}{% if page.dnd == true and page.categories contains {{ category }} %}* [{{ page.title }}]({{ site.baseurl }}{{ page.url }})
{% endif %}{% endfor %}

{% endfor %}


{% for cat in site.category-list %}
### {{ cat }}
<ul>
  {% for page in site.pages %}
    {% if page.dnd == true %}
      {% for pc in page.categories %}
        {% if pc == cat %}
          <li><a href="{{ page.url }}">{{ page.title }}</a></li>
        {% endif %} 
      {% endfor %}
    {% endif %}
  {% endfor %}
</ul>
{% endfor %} 