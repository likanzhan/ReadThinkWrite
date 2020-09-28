## Table of Contents

{% site.pages = site.pages | sort: "date", "last" %}
{% for page in site.pages %}
 - {{page.date}}: [{{page.title}}]({{site.url}}{{page.url}})
{% endfor %}