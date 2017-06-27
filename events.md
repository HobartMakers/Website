---
layout: default
title: Events
permalink: /events/
---

# Events


## Regular events

* Open nights are every Tuesday from 6pm - 9pm, and we welcome everyone!

* Side-projects Saturday is _usually_ every second Saturday afternoon. Double check in the [chatroom](https://riot.im/app/#/room/#hobartmakers:matrix.org) or check the [facebook events list](https://www.facebook.com/groups/hobartmakers/events/) to make sure. The goal is to bring an incomplete project and get some work done!

## National Science Week 2017

* We were lucky enough to receive funding to run a small event this year, we've chosen to demonstrate LoRa long range, low power radio - for connecting sensors to the Internet of Things. Check out our [National Science Week](/scienceweek/) page for more information.

## Upcoming Workshops

These are also listed on our [Facebook events list](https://www.facebook.com/groups/hobartmakers/events/) and our [TidyHQ events list](https://hobartmakers.tidyhq.com/public/schedule/events)

<table class="table">
 <thead>
   <tr>
   <td>Date</td>
   <td>Workshop</td>
   <td>Facilitator</td>
   </tr>
  </thead>
  <tbody>

{% for item in site.data.workshops %}
  {% unless item.archived %}
   <tr>
   <td>{{ item.date }}</td>
  {% if item.url %}
   <td><a href="{{ item.url }}" target="_blank">{{ item.workshop }}</a></td>
  {% else %}
   <td>{{ item.workshop }}</td>
  {% endif %}
   <td>{{ item.facilitator }}</td>
   </tr>
  {% endunless %}
{% endfor %}

  </tbody>
</table>


## Past Workshops

<table class="table">
 <thead>
   <tr>
   <td>Date</td>
   <td>Workshop</td>
   <td>Facilitator</td>
   </tr>
  </thead>
  <tbody>

{% for item in site.data.workshops %}
  {% if item.archived %}
   <tr style='text-decoration:line-through'>
   <td>{{ item.date }}</td>
  {% if item.url %}
   <td><a href="{{ item.url }}" target="_blank">{{ item.workshop }}</a></td>
  {% else %}
   <td>{{ item.workshop }}</td>
  {% endif %}
   <td>{{ item.facilitator }}</td>
   </tr>
  {% endif %}
{% endfor %}

  </tbody>
</table>

