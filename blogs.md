---
layout: page
title: Blogs
permalink: /blogs/
---


### Coming Soon!

<div class="row">
  <div class="col-sm-8">
  {% for post in site.posts %}
    {% if post.categories contains 'blogs' %}
      <div class="mb-5">
        <h2><a href="{{ post.url }}" class="text-decoration-none link-primary">{{ post.title }}</a></h2>
        <h6 class="date text-secondary">{{ post.date | date: "%A, %B %e, %Y" }}</h6>
        {{ post.excerpt }}
      </div>
    {% endif %}
  {% endfor %}
  </div>
  <!-- div class="col-sm-4">
    <h2>Upcoming Events</h2>
  </div -->
</div>