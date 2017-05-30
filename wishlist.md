---
layout: default
title: Wishlist
permalink: /wishlist/
---

<h3>Wishlist</h3>

<p>This is a general shopping list and wish list of things that anyone could help out with. The most important item is a larger space to set up and work in. The others are things we could buy new or second hand or build in some cases.</p>

<p>If you can help with any of this, please <a href="/contact/">get in touch</a></p>

<table class="table">
 <thead>
   <tr>
   <th>Item</th>
   <th>Notes</th>
   </tr>
 </thead>

<tbody>
{% for item in site.data.wishlist %}
{% if item.granted %}
   <tr style='text-decoration:line-through'>
{% else %}
   <tr>
{% endif %}
   <td>{{ item.item }}</td>
   <td>{{ item.notes }}</td>
   </tr>
{% endfor %}
</tbody>

</table>
