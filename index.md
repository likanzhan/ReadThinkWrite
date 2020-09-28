## Table of Contents

{% for page in site.pages %}
 - {{page.date}}-[{{page.title}}]({{site.url}}{{page.url}})
{% endfor %}