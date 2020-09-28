## Table of Contents

{% assign SortedPages = site.pages | sort: "date", "first" %}

{% for page in site.posts %}
 - {{page.date}}-{{page.author}}-[{{page.title}}]({{site.url}}{{page.url}})
{% endfor %}