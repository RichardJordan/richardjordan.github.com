---
layout: page
title: ...and another thing...
<!-- tagline: Supporting tagline -->
---
{% include JB/setup %}

<ul class="m-PostList">
  {% for post in site.posts %}
    <li class="c-ListItem-post clearfix">
      <div class="c-ListItem-postDate">
        {{ post.date | date_to_string }} &raquo; 
      </div>
      <div class="c-ListItem-postTitle">
        <a href="{{ BASE_PATH }}{{ post.url }}">
          {{ post.title }}
        </a>
      </div>
    </li>
  {% endfor %}
</ul>
