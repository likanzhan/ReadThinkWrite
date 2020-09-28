## 报告列表

{% assign SortedPages = site.pages | sort: "date", "first" %}

{% for page in site.posts %}
 - {{page.date | date: "%-d %B %Y" }}-{{page.author}}-[{{page.title}}]({{site.url}}{{page.url}})
{% endfor %}