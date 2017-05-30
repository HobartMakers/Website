---
layout: default
title: Equipment
permalink: /equipment/
---

<h3>Current Equipment</h3>

<p>We'll do our best to keep this list up to date, but if you notice anything out of date, please <a href="/contact/">get in touch</a></p>

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


