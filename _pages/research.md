---
title: ""
layout: archive
classes: wide
sitemap: true
permalink: /research/
author_profile: true
---

My research sits at the intersection of applied microeconomics and machine learning. I use explainable ML and causal inference to study poverty, wellbeing, and labour markets — below are my publications, working papers, and thesis.

## <i class="fas fa-book heading-icon"></i>Publications

<!-- Papers are defined once in _data/publications.yml and shared with the
     homepage's "Selected Research" section - update a paper there, not here. -->
<div class="cards" markdown="1">
{% for pub in site.data.publications %}
<div class="card" markdown="1" id="{{ pub.id }}">
<span class="card__tag">{{ pub.venue }}</span>

### {{ pub.title }}

{{ pub.abstract }}

<div class="tag-pills" markdown="1">
{% for tag in pub.tags %}<span class="tag-pill">{{ tag }}</span>
{% endfor %}</div>

<span class="card__cite">{{ pub.citation }}</span>
{% if pub.link_url and pub.link_url != "" %}
<div class="card__links" markdown="1">
[{{ pub.link_label }} &rarr;]({{ pub.link_url }}){: .inline-link target="_blank" rel="noopener noreferrer"}
</div>
{% endif %}
</div>
{% endfor %}
</div>

## <i class="fas fa-graduation-cap heading-icon"></i>Theses

<div class="cards" markdown="1">
<div class="card" markdown="1">
<span class="card__tag">PhD Dissertation &middot; University of Luxembourg &middot; 2023</span>

### Essays on the Prediction and Measurement of Individual Well-being

<span class="card__meta">Supervisor: Prof. Dr. Conchita D'Ambrosio</span>

<div class="tag-pills" markdown="1">
<span class="tag-pill">Machine Learning</span>
<span class="tag-pill">Vulnerability</span>
<span class="tag-pill">Poverty</span>
<span class="tag-pill">Wellbeing</span>
<span class="tag-pill">SOEP</span>
<span class="tag-pill">Material Deprivation</span>
<span class="tag-pill">SARS-CoV-2</span>
<span class="tag-pill">Individual Behaviour</span>
<span class="tag-pill">Explainable AI</span>
<span class="tag-pill">Policy Response</span>
<span class="tag-pill">EU-SILC</span>
</div>

<span class="card__cite">Taye, A. D. (2023). <em>Essays on the prediction and measurement of individual well-being</em> [Doctoral dissertation, University of Luxembourg]. ORBilu.</span>

<div class="card__links" markdown="1">
[View on ORBilu &rarr;](https://orbilu.uni.lu/handle/10993/55174){: .inline-link target="_blank" rel="noopener noreferrer"} &middot; 355 views &middot; 317 downloads
</div>
</div>
</div>
