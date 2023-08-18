---
layout: post
title: All spells
permalink: /spells/
---

<details markdown="1">
<summary><b>How spellcasting works</b></summary>
Some people can cast spells. They have <b>Magic Dice</b> (or <b>MD</b>) that they use to do so. For every <b>Magical</b>b> object the character has in their Inventory or Mind, they gain 1 Magic Dice, which is a d6. Some Gifts can also give Magic Dice.
  
<u><b>Casting a spell:</b></u> Whenever you cast a spell, you decide how many MD to invest in it, up to your maximum number of MD or 4, whichever is lower. The effects of the spell depend on the number of [dice] invested, as well as the [sum] of all results.

If an MD rolls a 6, you lose it, and can't use it anymire. Generally, classes recuperate lost MD after a good rest, although some of them don't.

Every time you roll doubles (the same result on 2 different dice), there's a <b>Mishap</b>.

<u><b>Mishaps:</b></u> These happen when you roll doubles when casting a spell. In this case, <b>something bad happens</b>, as determined by the GM. The effects of the mishap depend on the spell cast. Triples or quadruples are even worse. Mishaps can be something like making whatever it's supposed to fix worse, or fixing it in some unwanted way, or being cast on someone else, or fizzling, or damaging the caster, or...
</details>

<details markdown="1">
<summary><b>How to read a spell</b></summary>
  
<b>D:</b> the duration of the spell. You can only have 1 <i>concentration</i> spell active at the same time.

<b>T:</b> the potential target of the spell.

<b>R:</b> the casting range of the spell. Nearby is one room over. Far is 10 rooms over.

The effecs of the spell are written here. Sometimes, the effect is changed according to the number of [dice] used to cast the spell, or the [sum] of the results rolled by the used Magic dice.
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


