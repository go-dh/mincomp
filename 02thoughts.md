---
layout: page
title: Articles & Thought Pieces
permalink: /thoughts/
---

<div id="posts">
  <ul>
    {% for post in site.posts %}
	{% if post.category == "thoughts" %}
      <li><span>{{ post.date | date_to_string }}</span> - <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
	{% endif %}    
{% endfor %}
  </ul>
</div>