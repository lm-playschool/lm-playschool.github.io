---
layout: page
title: Accepted Papers
---

<div class="papers-section">

## Paper-only Track

<ul class="papers-list">

{% for paper in site.data.accepted_papers.paper_only %}
<li class="paper-entry">

<a class="paper-pdf-link" href="{{ paper.pdf | relative_url }}" target="_blank" rel="noopener" aria-label="Open PDF">![PDF]({{ "/assets/img/pdf-icon.svg" | relative_url }})</a>

<div class="paper-info">

### {{ paper.title }}

*{{ paper.authors }}*

{{ paper.abstract }}

</div>

</li>

{% endfor %}
</ul>

## Challenge Track

<ul class="papers-list">

{% for paper in site.data.accepted_papers.challenge %}
<li class="paper-entry">

<a class="paper-pdf-link" href="{{ paper.pdf | relative_url }}" target="_blank" rel="noopener" aria-label="Open PDF">![PDF]({{ "/assets/img/pdf-icon.svg" | relative_url }})</a>

<div class="paper-info">

### {{ paper.title }}

*{{ paper.authors }}*

{{ paper.abstract }}

</div>

</li>

{% endfor %}
</ul>

</div>
