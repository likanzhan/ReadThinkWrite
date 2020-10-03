{% for page in site.posts %}
{% assign author_size = page.author | size | minus: 3 %}
{% if author_size > 0 %}
{% assign ToAppend = "LL" %}
{% else %}
{% assign ToAppend = "S" %}
{% endif %}
{% assign author =  page.author | append: ToAppend %}
 - {{page.date | date: "%Y-%m-%d" }}-{{page.author}} - {{author}} -[{{page.title}}]({{site.url}}{{page.url}})
{% endfor %}