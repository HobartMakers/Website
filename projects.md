---
layout: default
title: Projects
permalink: /projects/
---

<h3>Projects</h3>

<p>Here's an idea of what we're working on, and things we probably need help with.</p>

<p>If you want to know more, or want to volunteer some time and effort, please <a href="/contact/">get in touch</a> or let us know at an open night meetup.</p>

<p>If you're working on something at the space, or for the space, and we've left you off this list, please <a href="/contact/">let us know</a></p>

<table class="table">
 <thead>
   <tr>
   <th>Project</th>
   <th>Lead</th>
   <th>Goal</th>
   <th>Status</th>
   </tr>
  </thead>
  <tbody>

{% for item in site.data.projects %}
   <tr>
   <td>{{ item.project }}</td>
   <td>{{ item.lead }}</td>
   <td>{{ item.description }}</td>
   <td>{{ item.status }}</td>
   </tr>
{% endfor %}

  </tbody>
</table>


