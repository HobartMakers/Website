---
layout: default
title: Welcome
permalink: /
members: 17
---

# {{ page.title }}

<div class="pull-right" style="max-width:600px; padding-bottom:30px; margin-left:10px; margin-right:10px;">
<ul class="rslides">

{% for item in site.data.slides %}

  <li>
  {% if item.url %}
  <a href="{{ item.url }}">
  {% endif %}
  <img src="{{ item.img }}" alt="{{ item.caption }}">
  {% if item.url %}
  </a>
  {% endif %}
  <p class="caption">{{ item.caption }}</p>
  </li>

{% endfor %}

</ul>
</div>

We are a group of people that love [making](https://en.wikipedia.org/wiki/Maker_culture) things. We are based in Hobart, Tasmania and we welcome people of any age, gender, skill level and from any background.

We are run by a team of five (Craig, Scott, Michael, Paul and Mary). Overall, we have {{ page.members }} members and counting. Please [join us](https://hobartmakers.tidyhq.com/public/memberships/new)! :smiley:

To find out more:

* Come to an [event](/events) - Open night is on Tuesday evenings.
* Reach us via the [contact](/contact) page
* or take a look at our [FAQ](/faq)

