---
layout: page
title:
permalink: /tech/
---


<div class="posts">
  {% for post in site.posts %}
      {% if post.tags contains 'Technology' %}
      <article class="post">
        <h2>
          <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
        </h2>
      </article>
      {% endif %}
  {% endfor %}
</div>
