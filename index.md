## Table of Contents

{{ site.pages | sort: "date", "last" }}
{% for page in site.pages %}
 - {{page.date}}-{{page.author}}-[{{page.title}}]({{site.url}}{{page.url}})
{% endfor %}