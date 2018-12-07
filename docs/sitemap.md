---
---
### Version 1.1

{% for category in site.categories %}
#{{category}}
{% for page in site.pages %}{% if page.dnd == true and page.categories contains {{ category }} %}* [{{ page.title }}]({{ site.baseurl }}{{ page.url }})
{% endif %}{% endfor %}

{% endfor %}