{% for page in site.posts %}
{% assign author_size = page.author | size | minus: 3 %}
 - {{page.date | date: "%Y-%m-%d" }}-{{page.author}} - {{author_size}} -[{{page.title}}]({{site.url}}{{page.url}})
{% endfor %}