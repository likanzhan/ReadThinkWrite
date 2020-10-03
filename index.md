{% for page in site.posts %}

 - {{page.date | date: "%Y-%m-%d" }}-{{page.author}}-[{{page.title}}]({{site.url}}{{page.url}})

{% endfor %}