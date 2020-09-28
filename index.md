## Table of Contents

{% for page in {{ site.pages | sort: "date", "last" }} %}
 - {{page.date}}: [{{page.title}}]({{site.url}}{{page.url}})
{% endfor %}