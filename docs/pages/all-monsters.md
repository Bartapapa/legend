---
layout: post
title: All monsters
permalink: /monsters/all
---

{% capture posts %}
  {% for post in site.tags.monster %}
    |{{ post.title }}#{{ post.url }}
  {% endfor %}
{% endcapture %}
{% assign sortedposts = posts | split: '|' | sort %}
<ol>
{% for post in sortedposts %}
{% assign postitems = post | split: '#' %}
{% unless forloop.first %}
  <li> <a href="{{ site.baseurl }}{{ postitems[1] }}">{{ postitems[0] }}</a></li> 
{% endunless %}
{% endfor %} 
</ol>
