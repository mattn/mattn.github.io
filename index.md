---
layout: page
---
{% include JB/setup %}

{% for post in site.posts %}
<h3><a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></h3>
<span>{{ post.date | date: "%Y/%m/%d" }}</span>

{{ post.content }}

<br />
{% endfor %}
