---
layout: page
title: The Leiboff Lab
permalink: /thelab/
---

People
==================
<div>
  {% for current_people in site.current_people %}
      <div style="overflow: hidden;">
        {% if current_people.profile-image %}
        {% include people-profile-image.html image=current_people.profile-image alt=current_peopleprofile-image-alt %}
        {% endif %}
      <h2><a href="{{ current_people.url }}">{{ current_people.name }}</a></h2>
      <h3>{{ current_people.position }}</h3>
      <p>{{ current_people.content | markdownify }}</p></div>
  {% endfor %}
</div>

<!-- 
Places
==================

Things
================== -->
