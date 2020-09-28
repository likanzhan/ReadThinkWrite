## Table of Contents

{% assign SortedPages = site.pages | sort: "date", "first" %}

{% for page in site.pages %}
{% assign PageType = page | split: "." %}
{% if PageType.last == "md" %}
 - {{page.date}}-{{page.author}}-[{{page.title}}]({{site.url}}{{page.url}})
{% endif %}
{% endfor %}