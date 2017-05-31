---
layout: default
title: Photos
permalink: /photos/
---

# {{ page.title }}


<div class="row">

{% for item in site.data.photos %}

 <div class="col-sm-6 col-md-4">
  <div class="thumbnail">
   <a href="{{ item.img }}" data-lightbox="all-photos" data-title="{{ item.caption }}">
   <img src="{{ item.img }}" alt="{{ item.caption }}" title="{{ item.caption }}">
   </a>
  </div>
 </div>

{% endfor %}

</div>


