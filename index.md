## 报告列表

{% assign SortedPages = site.pages | sort: "date", "first" %}

{% for page in site.posts %}
 - {{page.date | date: "%Y-%m-%d" }}-{{page.author}}-[{{page.title}}]({{site.url}}{{page.url}})
{% endfor %}