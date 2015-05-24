---
layout: page
title: Challenges
permalink: /challenges/
---

<div id="posts">
  <ul>
    {% for post in site.posts %}
	{% if post.category == "challenge" %}
      <li><span>{{ post.date | date_to_string }}</span> - <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
	{% endif %}    
{% endfor %}
  </ul>
</div>