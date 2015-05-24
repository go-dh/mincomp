---
layout: page
title: Links & Resources
permalink: /resources/
---

<div id="posts">
  <ul>
    {% for post in site.posts %}
	{% if post.category == "resource" %}
      <li><span>{{ post.date | date_to_string }}</span> - <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
	{% endif %}    
{% endfor %}
  </ul>
</div>