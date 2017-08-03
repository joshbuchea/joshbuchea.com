---
layout: default
title: Posts
---

<div class="archive">
  {% for post in site.posts limit:50 %}
    <div class="archive-item">
      <span class="post-date archive-date">{{ post.date | date: "%B %-d, %Y" }}</span>
      <a class="archive-title" href="{{ post.url }}">{{ post.title }}</a>
    </div>
  {% endfor %}
</div>

<!--

<div class="archive">
  {% for post in site.posts %}
    {% capture currentyear %}{{ post.date | date: "%Y" }}{% endcapture %}
    {% if currentyear != year %}
      <h2 class="archive-year">{{ currentyear }}</h2>
      {% capture year %}{{ currentyear }}{% endcapture %}
    {% endif %}
    <div class="archive-item">
      <span class="post-date archive-date">{{ post.date | date: "%B %-d, %Y" }}</span>
      <a class="archive-title" href="{{ post.url }}">{{ post.title }}</a>
    </div>
  {% endfor %}
</div>

-->
