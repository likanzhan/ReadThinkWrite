## Table of Contents

{% for page in site.pages %}
 - {{page.date}}-{{page.author}}-[{{page.title}}]({{site.url}}{{page.url}})
{% endfor %}