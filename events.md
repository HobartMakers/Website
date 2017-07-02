---
layout: default
title: Events
permalink: /events/
---

## Upcoming Events

Open nights and Saturday Crafternoons are open to all, and we'd love you to come and join us. Workshops do require a paid ticket. To purchase, please follow the links provided.

<!--Event data is also available in an ICS file [here](https://hobartmakers.com/calendar.ics) -->

<table class="table">
 <thead>
   <tr>
   <td style="width:15%">Date</td>
   <td style="width:15%">Time</td>
   <td style="width:30%">Title</td>
   <td style="width:20%">Facilitator</td>
   <td style="width:20%">Notes</td>
   </tr>
  </thead>
  <tbody>

{% capture nowunix %}{{ 'now' | date: '%s' }}{% endcapture %}
{% assign nowunix = nowunix | plus: 0 %}

{% for item in site.data.workshops %}

  {% capture posttime %}{{ item.start | date: '%s' }}{% endcapture %}
  {% assign posttime = posttime | plus: 0 %}

  {% if posttime >= nowunix %}
   <tr>
   <td>{{ item.start | date: '%a, %-d %b %Y'}}</td>
   <td>{{ item.start | date: '%l:%M%P' }} - {{ item.end | date: '%l:%M%P'}}</td>
  {% if item.url %}
   <td><a href="{{ item.url }}" target="_blank">{{ item.workshop }}</a></td>
  {% else %}
   <td>{{ item.workshop }}</td>
  {% endif %}
   <td>{{ item.facilitator }}</td>
   <td>{{ item.notes }}</td>
   </tr>
  {% endif %}
{% endfor %}

  </tbody>
</table>


## Past Events

<table class="table">
 <thead>
   <tr>
   <td style="width:15%">Date</td>
   <td style="width:15%">Time</td>
   <td style="width:30%">Title</td>
   <td style="width:20%">Facilitator</td>
   <td style="width:20%">Notes</td>
   </tr>
  </thead>
  <tbody>

{% for item in site.data.workshops reversed %}

  {% capture posttime %}{{ item.start | date: '%s' }}{% endcapture %}
  {% assign posttime = posttime | plus: 0 %}

  {% if posttime < nowunix %}
   <!--tr style='text-decoration:line-through'-->
   <tr>
   <td>{{ item.start | date: '%a, %-d %b %Y'}}</td>
   <td>{{ item.start | date: '%l:%M%P' }} - {{ item.end | date: '%l:%M%P'}}</td>
  {% if item.url %}
   <td><a href="{{ item.url }}" target="_blank">{{ item.workshop }}</a></td>
  {% else %}
   <td>{{ item.workshop }}</td>
  {% endif %}
   <td>{{ item.facilitator }}</td>
   <td>{{ item.notes }}</td>
   </tr>
  {% endif %}
{% endfor %}

  </tbody>
</table>

