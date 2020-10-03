{% for page in site.posts %}
{% assign author_size = page.author | size | minus: 3 %}
{% if author_size == 1 %}
{% assign author = "L" %}
{% else %}
{% assign author = "SS" %}
{% endif %}
 - {{page.date | date: "%Y-%m-%d" }}-{{page.author}}-{{author}}-{{author_size}}-[{{page.title}}]({{site.url}}{{page.url}})
{% endfor %}