---
layout: page
title: Links & Resources
permalink: /resources/
---

<div id="posts">
  <ul>
    {% for post in site.posts %}
	{% if post.category == "resource" %}
      <li><a href="{{ post.link }}" target="_blank">{{ post.title }}</a> by <span class="italic">{{ post.author }}</span></li> 
      <p class="blurb">{{ post.blurb }}</p>
	{% endif %}    
{% endfor %}
  </ul>
</div>