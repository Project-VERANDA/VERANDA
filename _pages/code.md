---
layout: archive
title: "Code"
permalink: /code/
author_profile: false
read_more: disabled
classes: wide
---

<div class = "text-justify">
Explore open source code originated from the VERANDA project or related activities. A button below each publication links to a github repository or related website. The list will grow with time as new advances are being made.  
</div>
<p></p>

{% if paginator %}
  {% assign code = paginator.code | reverse %}
{% else %}
  {% assign code = site.code | reverse %}
{% endif %}

{% for post in code %}
  {% include archive-single.html %}
  <p></p>
{% endfor %}
