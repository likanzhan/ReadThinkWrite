{% for page in site.posts %}
{% assign author_size = page.author | size | minus: 3 %}
{% if author_size == 0 %}
 - {{page.date | date: "%Y-%m-%d" }}-{{page.author}}-[{{page.title}}]({{site.url}}{{page.url}})
{% else %}
 - {{page.date | date: "%Y-%m-%d" }}-{{page.author | append: " "}}-[{{page.title}}]({{site.url}}{{page.url}})
{% endif %}
{% endfor %}