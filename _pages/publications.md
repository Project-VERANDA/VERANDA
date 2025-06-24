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

<hr>

<p>
  <b>Published</b>
</p>
  <p>
  <a href="https://aclanthology.org/2025.coling-main.77/">Wang, Q., Anikina, T., Feldhus, N., Ostermann, S., Möller, S. and Schmitt, V., 2025, January. Cross-Refine: Improving Natural Language Explanation Generation by Learning in Tandem. In Proceedings of the 31st International Conference on Computational Linguistics (pp. 1150-1167).</a>
  </p>
  <p>
  <a href="https://doi.org/10.18653/v1/2024.findings-emnlp.76">Wang, Q., Anikina, T., Feldhus, N., Ostermann, S. and Möller, S., 2024, November. CoXQL: A Dataset for Parsing Explanation Requests in Conversational XAI Systems. In Findings of the Association for Computational Linguistics: EMNLP 2024 (pp. 1410-1422).</a>
  </p>
  <p>
  <a href="https://doi.org/10.18653/v1/2024.findings-emnlp.76">Flanagan, L. and Poikela, M., 2025. Attitudes of Developers Towards Privacy in Personal Health Applications. Studies in health technology and informatics, 327, pp.949-953.</a>
  </p>
<br>
<p>
<b>In Press</b>
</p>
  <p>
  <a href="https://arxiv.org/abs/2501.00777">Wang, Q., Feldhus, N., Ostermann, S., Villa-Arenas, L.F., Möller, S. and Schmitt, V., 2025. FitCF: A Framework for Automatic Feature Importance-guided Counterfactual Example Generation. arXiv preprint arXiv:2501.00777.</a>
  </p>
  <p>
  <a href="https://arxiv.org/abs/2501.00777">Dhaini, M., Erdogan, E., Feldhus, N. and Kasneci, G., 2025. Gender Bias in Explainability: Investigating Performance Disparity in Post-hoc Methods. arXiv preprint arXiv:2505.01198.</a>
  </p>
  <p>
  <a href="https://arxiv.org/abs/2501.00777">Franzreb, C., Das, A., Polzehl, T. and Möller, S., 2025. Private kNN-VC: Interpretable Anonymization of Converted Speech. arXiv preprint arXiv:2505.17584.</a>
  </p>
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
