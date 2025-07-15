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

<b>In Press</b>
</p>
<p>
  Speech Anonymizer: <a href="https://github.com/carlosfranzreb/private_knnvc">https://github.com/carlosfranzreb/private_knnvc</a></p>

<p style="text-indent: 40px"> Associated paper: <a href="https://arxiv.org/abs/2501.00777">Franzreb, C., Das, A., Polzehl, T. and Möller, S., 2025. Private kNN-VC: Interpretable Anonymization of Converted Speech. arXiv preprint arXiv:2505.17584.</a>
</p>
  
{% if paginator %}
  {% assign code = paginator.code | reverse %}
{% else %}
  {% assign code = site.code | reverse %}
{% endif %}

{% for post in code %}
  {% include archive-single.html %}
  <p></p>
{% endfor %}
