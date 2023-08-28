---
layout: post
title: All spells
permalink: /spells/
---

<details markdown="1">
<summary><b>How spellcasting works</b></summary>
If you have a <b>Spellbook</b>, you can cast the associated spell. You can roll up to 4 Magic dice (that you acquire by holding <i>magical</i> items in your Inventory). The effects of the spell depend on the number of [dice] used, and the [sum] of the result.

If you roll doubles when casting a spell, you mark 1 <b>Notch</b> on it. You can only repair it by <b>Recharging</b> it. If it gets 3 Notches, it is destroyed and is unrepairable.

If you roll doubles when casting a spell without a spellbook (such as with the Spellmind gift), then you take 1d6 Wit damage. Make a Wit save - if unsuccessful, you get the <b>Mad</b> Condition, that can be removed after a full rest. This takes up a slot.
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


