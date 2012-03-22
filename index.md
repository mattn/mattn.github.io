---
layout: page
tagline: Supporting tagline
---
{% include JB/setup %}

{% for post in site.posts %}
<h3><a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></h3>
<span>{{ post.date | date_to_string }}</span>

{{ post.content }}

<br />
{% endfor %}
