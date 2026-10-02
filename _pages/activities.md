---
title: "Academic Activities"
layout: archive
classes: wide
sitemap: true
permalink: /activities/
author_profile: true
toc: true
toc_label: "Category"
toc_icon: "gear"
---

## <i class="fas fa-users heading-icon"></i>Selected Conferences & Workshops

<div class="honor-list" markdown="1">
<div class="honor-row" markdown="1">
<span class="honor-row__year">Aug 2022</span>
<span class="honor-row__text">IARIW 37th General Conference, Luxembourg</span>
</div>
<div class="honor-row" markdown="1">
<span class="honor-row__year">Jun 2022</span>
<span class="honor-row__text">Well-Being 2022 Conference, STATEC, Luxembourg</span>
</div>
<div class="honor-row" markdown="1">
<span class="honor-row__year">Apr 2022</span>
<span class="honor-row__text">The 14th Workshop on Labour Economics – IAAEU, University of Trier</span>
</div>
<div class="honor-row" markdown="1">
<span class="honor-row__year">Apr 2022</span>
<span class="honor-row__text">Brownbag Seminar, STATEC-Research, Luxembourg</span>
</div>
<div class="honor-row" markdown="1">
<span class="honor-row__year">Jun 2019</span>
<span class="honor-row__text">Inequality by the Numbers Workshop, CUNY Graduate Center, New York</span>
</div>
</div>

## <i class="fas fa-school heading-icon"></i>Summer Schools

<div class="honor-list" markdown="1">
<div class="honor-row" markdown="1">
<span class="honor-row__year">Sep 2022</span>
<span class="honor-row__text">Causal Analysis and Machine Learning, University of Oxford, Oxford</span>
</div>
<div class="honor-row" markdown="1">
<span class="honor-row__year">Sep 2019</span>
<span class="honor-row__text">Explainable Data Science, European Association for Data Science (EuADS)</span>
</div>
</div>

## <i class="fas fa-building heading-icon"></i>Research Visits

<div class="honor-list" markdown="1">
<div class="honor-row" markdown="1">
<span class="honor-row__year">2019</span>
<span class="honor-row__text">STATEC-Research, Luxembourg (May – August)</span>
</div>
<div class="honor-row" markdown="1">
<span class="honor-row__year">2008</span>
<span class="honor-row__text">Ethiopian Economics Association, Addis Ababa, Ethiopia (June – August)</span>
</div>
</div>

## <i class="fas fa-globe-africa heading-icon"></i>Places I have been

{% assign places = site.data.visited_places %}
{% assign continents = places | map: "continent" | uniq %}
{% assign city_total = 0 %}
{% for p in places %}{% assign city_total = city_total | plus: p.cities.size %}{% endfor %}

<div class="stat-bar" markdown="1">
<div class="stat" markdown="1">
<span class="stat__number">{{ continents.size }}</span>
<span class="stat__label">Continents</span>
</div>
<div class="stat" markdown="1">
<span class="stat__number">{{ places.size }}</span>
<span class="stat__label">Countries</span>
</div>
<div class="stat" markdown="1">
<span class="stat__number">{{ city_total }}</span>
<span class="stat__label">Cities</span>
</div>
</div>
