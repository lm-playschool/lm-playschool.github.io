---
layout: page
title: Accepted Papers
---

<div class="papers-section">

<h2>Paper-only Track</h2>
{% for paper in site.data.accepted_papers.paper_only %}
<div class="paper-entry">
  <div class="paper-info">
    <h3 class="paper-title">{{ paper.title }}</h3>
    <p class="paper-authors">{{ paper.authors }}</p>
    <p class="paper-abstract">{{ paper.abstract }}</p>
  </div>
  <a class="paper-pdf-link" href="{{ paper.pdf | relative_url }}" target="_blank" rel="noopener" aria-label="Open PDF">
    {% include pdf-icon.html %}
  </a>
</div>
{% endfor %}

<h2>Challenge Track</h2>
{% for paper in site.data.accepted_papers.challenge %}
<div class="paper-entry">
  <div class="paper-info">
    <h3 class="paper-title">{{ paper.title }}</h3>
    <p class="paper-authors">{{ paper.authors }}</p>
    <p class="paper-abstract">{{ paper.abstract }}</p>
  </div>
  <a class="paper-pdf-link" href="{{ paper.pdf | relative_url }}" target="_blank" rel="noopener" aria-label="Open PDF">
    {% include pdf-icon.html %}
  </a>
</div>
{% endfor %}

</div>
