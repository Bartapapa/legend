---
layout: post
title: Monsters by habitat
permalink: /monsters/monsters-by-habitat
---

## Any

> Pretty much any environment. Migrating monsters, colonizers and the like.

{% capture posts %}
  {% for post in site.tags.any %}
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

## Aquatic

> Bodies of water, ponds, oceans, sometimes acid lakes

{% capture posts %}
  {% for post in site.tags.aquatic %}
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

## Coastal

> Estuaries, deltas, lakeshores, beaches and the like.

{% capture posts %}
  {% for post in site.tags.coastal %}
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

## Desert

> Hot, arid areas, such as sandy deserts, shrublands and the like.

{% capture posts %}
  {% for post in site.tags.desert %}
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

## Forest

> Woody areas such as boreal, tropical or temperate forests, and certain marshlands.

{% capture posts %}
  {% for post in site.tags.forest %}
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

## Hill

> Areas with slopes and valleys.

{% capture posts %}
  {% for post in site.tags.hill %}
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

## Mountain

> Great mountains, chains, mesas and hoodoos.

{% capture posts %}
  {% for post in site.tags.mountain %}
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

## Plain

> Great spreads of flat land, such as meadows, clearings and the like.

{% capture posts %}
  {% for post in site.tags.plain %}
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

## Swamp

> Swampy, muddy areas such as bogs, marshes and fens.

{% capture posts %}
  {% for post in site.tags.swamp %}
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

## Underground

> Tight, dark warrens, such as tunnels, caves and pits.

{% capture posts %}
  {% for post in site.tags.underground %}
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
