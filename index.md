---
layout: default
title: Home
---
<div class="row">
  <div class="col-md-8">
    <h1>{{ site.title }}</h1>
    <p>{{ site.description }}</p>

    <h2>Latest posts</h2>
    <ul>
    {% for post in site.posts %}
      <li><a href="{{ post.url | relative_url }}">{{ post.title }}</a> — <small>{{ post.date | date: "%b %d, %Y" }}</small></li>
    {% endfor %}
    </ul>
  </div>

  <aside class="col-md-4">
    <h4>About</h4>
    <p>{{ site.author.name }}</p>
  </aside>
</div>
