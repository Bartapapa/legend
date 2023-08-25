---
layout: post
title: All spells
permalink: /spells/
---

<details markdown="1">
<summary><b>How spellcasting works</b></summary>
If you have a <b>Spellbook</b>, you can cast the associated spell. Roll Wit and add a d6. The effects of the spell depend on the [sum] of the results, the [size] of the biggest die, and the [degrees] of success.
  
On a failure, the spell cannot be cast any more for the day, and needs to be recharged (stated in the spell). If you roll doubles, a <b>Mishap</b> occurs along with the usual effects. The GM determines what happens according to the spell and situation.

</details>

***

{% capture posts %}
  {% for post in site.tags.spell %}
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


