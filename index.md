---
layout: page
title: Welcome
---
{% include JB/setup %}

My name is Kanit Wongsuphasawat.  I am building my portfolio on github.com
    

<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>


