---
layout: page
title: Thought Pieces
permalink: /thoughts/
---

<div id="posts">
  <ul>
    {% for post in site.posts %}
	{% if post.category == "thoughts" %}
      <li><span>{{ post.date | date_to_string }}</span> - <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a> by <span class="italic">{{ post.author }}</span></li>
	{% endif %}    
{% endfor %}
  </ul>
</div>