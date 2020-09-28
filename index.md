## Table of Contents

 {% assign SortedPosts = site.posts | sort: "date", "first" %}
{% for page in SortedPosts %}
 - {{page.date}}-{{page.author}}-[{{page.title}}]({{site.url}}{{page.url}})
{% endfor %}