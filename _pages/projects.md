---
layout: archive
title: "Projects"
permalink: /projects/
author_profile: false
read_more: disabled
classes: wide

sidebar: 
 nav: sidebar-projects
---

{% if paginator %}
  {% assign posts = paginator.posts %}
{% else %}
  {% assign projects = site.projects %}
{% endif %}

{% for post in projects reversed %}
  {% include archive-single.html %}
  <p></p>
{% endfor %}