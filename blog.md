---
layout: page
title: Blog
---

<ul>
  {% for post in site.posts %}
    <li>
      <span>{{ post.date | date: "%b %-d, %Y" }}</span>

      <a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>
