---
layout: home
permalink:
---

<h1>Blog Posts</h1>

<ul>
  {% assign sorted_posts = site.posts | sort: 'date' %}
  {% for post in sorted_posts %}
    <p>
      <a href="{{ post.url }}">{{ post.title }}</a> - {{ post.date | date: "%B %d, %Y" }}
    </p>
  {% endfor %}
</ul>
