---
layout: project
title: words
permalink: /blog/
order: 2
---

<ul class="post-list">
  {% for post in site.posts %}
    {% if post.status != 'draft' %}
    <li>
      <div class="post-links">
         <a href="{{ post.url | prepend: site.baseurl }}"> {{ post.title }} </a>
      </div>
    </li>
    {% endif %}
  {% endfor %}
</ul>
