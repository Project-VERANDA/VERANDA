---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: false
read_more: disabled
classes: wide
---

<div class = "text-justify">
Explore publications originated from the VERANDA project or related activities. If available, a button below each publication links to a PDF version of the full article or excerpt. The list will grow with time as new advances are being made.  
</div>
<p></p>

{% if paginator %}
  {% assign posts = paginator.posts | reverse %}
{% else %}
  {% assign publications = site.publications | reverse %}
{% endif %}

{% for post in publications %}
  {% include archive-single.html %}
  <p></p>
{% endfor %}
