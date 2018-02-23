---
layout: page
title: Blog
---

<ul class="o-list-bare">
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
      <span>({{ post.date | date: "%b %-d, %Y" }})</span>
    </li>
  {% endfor %}
</ul>
