---
layout: page
title: Tutorials
permalink: /tutorials/
---

<div id="posts">
  <ul>
    {% for post in site.posts %}
	{% if post.category == "tutorial" %}
      <li><span>{{ post.date | date_to_string }}</span> - <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
	{% endif %}    
{% endfor %}
  </ul>
</div>