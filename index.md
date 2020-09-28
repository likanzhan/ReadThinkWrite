## Table of Contents

 {% assign SortedPages = site.pages | sort: "date", "last" %}
{% for page in SortedPages %}
 - {{page.date}}-{{page.author}}-[{{page.title}}]({{site.url}}{{page.url}})
{% endfor %}