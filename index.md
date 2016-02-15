---
layout: top
permalink: /
---
<div class="posts">
  <h3>記事一覧</h3>

  <ul class="entry-list">
    {% for post in site.posts %}
    <li>
    <div class="entry-head">
      <span class="entry-label">{{ post.date | date: "%Y/%m/%d" }}&nbsp;&raquo;&nbsp;</span>
      <span class="entry-title"><a href="{{ post.url }}">{{ post.title }}</a></span>
    </div>
    <div class="entry-digest">{{ post.content | strip_html | strip_newlines | truncatewords: 10 }}</div>
    </li>
    {% endfor %}
  </ul>
</div>

<div class="links">

  <div class="link-block">
    <h3>連絡先など</h3>
    <a href="https://github.com/mattn/">GitHub</a><br />
    <a href="https://twitter.com/mattn_jp/">Twitter</a><br />
    <a href="http://mattn.kaoriya.net/">Blog</a><br />
  </div>

</div>

<div class="footer">
  <a class="small" href="mailto:mattn.jp@gmail.com">mattn.jp@gmail.com</a>
</div>
