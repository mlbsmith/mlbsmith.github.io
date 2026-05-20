---
layout: page
title: Writing
permalink: /writing/
---

<div class="posts">
  {% for post in site.posts %}
    <article class="post">
      <h2><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h2>
      <div class="date">{{ post.date | date: "%B %d, %Y" }}</div>
      {{ post.excerpt }}
    </article>
  {% endfor %}
</div>
