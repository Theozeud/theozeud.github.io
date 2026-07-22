---
layout: page
title: Publications
subtitle: Preprints and publications.
slug: publications
permalink: /publications/
---

<ul class="publications">
  {% for paper in site.data.publications %}
  <li class="publications__item{% if paper.placeholder %} publications__item--placeholder{% endif %}">
    <p class="publications__title">{{ paper.title }}</p>
    <p class="publications__authors">{{ paper.authors }}</p>
    <p class="publications__venue">{{ paper.venue }}{% if paper.year %}, {{ paper.year }}{% endif %}</p>
    {% if paper.links %}
    <p class="publications__links">
      {% if paper.links.arxiv %}<a href="{{ paper.links.arxiv }}">arXiv</a>{% endif %}
      {% if paper.links.pdf %}<a href="{{ paper.links.pdf }}">PDF</a>{% endif %}
      {% if paper.links.doi %}<a href="{{ paper.links.doi }}">DOI</a>{% endif %}
      {% if paper.links.code %}<a href="{{ paper.links.code }}">Code</a>{% endif %}
    </p>
    {% endif %}
  </li>
  {% endfor %}
</ul>
