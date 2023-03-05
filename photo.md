---
layout: page
title: photos
permalink: /photo/
---
<style>
    img.photo-list
{
	width: 256px;
	height: 196px;
	object-fit: cover;
    padding: 3px;
}

</style>

<h3> Click on each photo to see more </h3>


{% for item in site.photos %}
<div class="row">
  <div class="column">
    <p><a href="{{ item.url }}"><img class="photo-list" src='{{ {{item.photos[0].thumb }}' ></a></p>
  </div>
</div>
{% endfor %}