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

<u><b>Mishaps:</b></u> These happen when you roll doubles when casting a spell. In this case, <b>something bad happens</b>, as determined by the [sum]. The effects of the mishap depend on the spell cast. Mishaps can be something like making whatever it's supposed to fix worse, or fixing it in some unwanted way, or being cast on someone else, or fizzling, or damaging the caster, or...
</details>

<details markdown="1">
<summary><b>Mishaps</b></summary>
<small>Adapted from Cairn's rules for [GLOG magic](https://cairnrpg.com/hacks/glog-magic/)</small>

| Mishap [sum] |                   |
|:-------------|:------------------|
| 2            | You can't use cast Spells for 1d6 hours. Any attempt to manipulate magic fails.                  |
| 3            | For the next 24 hours, you lose MD on a 4+ instead of just a 6.                  |
| 4            | There is a chain reaction to the Spell. The GM says how.                 |
| 5            | The Spell's effects are reversed. The GM says how.                 |
| 6            | Any objects in your Inventory that are not fireproof combust. You're immune to fire for short bursts.                  |
| 7            | You are reduced to 0 HP. You can't regain HP in any way for 24 hours.                  |
| 8            |                   |
| 9            |                   |
| 10           | You become insubstantial for 1d6 hours as your spirit leaves your body, which remains helpless and unconscious. You can pass through walls, but can't physically act with anything. No one can hear or see you through mundane means.                 |
| 11           | You suffer horrid burns. Lose 1d6 max HP. Every time you cast a spell, you can add an additional MD (different color). If this MD is lost, you lose 1 max HP.                  |
| 12           | You permanently lose 1 MD. Ethereal floating magic around you constantly gives you 1 Armor.                  |
| 13           | If you cast the spell from a Spellbook, the spellbook is destroyed. Otherwise, lose the spell from your Mind.                  |
| 14           | Whenever you lose an MD, gain a Spell Tumor, that can either take up a slot in your Inventory or Mind. Only specialized healers can remove these.                  |
| 15           |                   |
| 16           | You lose 1 Might permanently as the spell tears out plantlife around you, reconstructing you as best it can. You have 1 Armor, however take increased damage from fire (+1 damage per dice)                  |
| 17           | You are transformed into something weird and unnatural. The GM describes it. You're still you, but...                  |
| 18           |                   |
| 19           | You exchange one of your limbs from some extraterrestrial creature, and gain all its benefits as well as drawbacks. The GM knows, but you don't necessarily. Also - it's coming for you, and it's mad as hell.                  |
| 20           | An extradimensional entity notices fragments of your arcane turbulence. The GM rolls a Reaction roll to determine how it reacts to you. You'll meet it in 7 days.                  |
| 21           | You become a vessel of pure arcane energy - you need not sleep, drink or eat, or even breathe. Whenever you would lose MD, you instead lose 1 Might. When you have 0 Might left, you become a spell. The GM determines which.                  |
| 22           | You create an exact duplicate of yourself. One becomes older, the other becomes younger. They age at the rate of one year pper day. If one dies, the other does too. If ever you combine, you gain +2 to all base attributes.                  |
| 23           | You become an Elemental. Create a True Name for yourself. Magical energies surround you, and mundane attacks against you are useless. If someone learns your True Name, they can control you. Other Elementals will come for you, to bring you back into their dimension.                  |
| 24           |                   |
| 25+          |                   |

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


