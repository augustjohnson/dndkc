---
---
{% for page in site.pages %}
* [{{ page.title }}]({{ site.baseurl }}/{{ page.url }})
{% endfor %}


{% for page in site.pages %}



{% for page in site.pages %}{% if page.dnd == true and page.categories contains "faction" %}<a href="{{site.baseurl}}{{ page.url }}">{{ page.title }}</a> | {{page.alignment}}
{% endif %}{% endfor %}

{% for category in site.pages[categories] %}
#{{category}}
{% for page in site.pages %}{% if page.dnd == true and page.categories contains {{category}} %}* [{{page.title}}]({{site.baseurl}}{{page.url}})
{% endif %}{% endfor %}

{% endfor %}