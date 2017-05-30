---
layout: default
title: Equipment
permalink: /equipment/
---

### Current Equipment

<table class="table">
 <thead>
   <tr>
   <th>Item</th>
   <th>Go to person</th>
   <th>Status</th>
   </tr>
  </thead>
  <tbody>

{% for item in site.data.equipment %}
   <tr>
   <td>{{ item.name }}</td>
   <td>{{ item.person }}</td>
   <td>{{ item.status }}</td>
   </tr>
{% endfor %}

  </tbody>
</table>

### Wishlist

| Item                          |
|-------------------------------|
| Digital Oscilloscope          |


