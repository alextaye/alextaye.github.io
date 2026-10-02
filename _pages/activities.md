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

<div class="timeline" markdown="1">
<div class="timeline__item" markdown="1">
<span class="timeline__date">August 2022</span>
<div class="timeline__title">IARIW 37th General Conference</div>
<div class="timeline__org">Luxembourg</div>
</div>
<div class="timeline__item" markdown="1">
<span class="timeline__date">June 2022</span>
<div class="timeline__title">Well-Being 2022 Conference</div>
<div class="timeline__org">STATEC, Luxembourg</div>
</div>
<div class="timeline__item" markdown="1">
<span class="timeline__date">April 2022</span>
<div class="timeline__title">The 14th Workshop on Labour Economics – IAAEU</div>
<div class="timeline__org">University of Trier</div>
</div>
<div class="timeline__item" markdown="1">
<span class="timeline__date">April 2022</span>
<div class="timeline__title">Brownbag Seminar</div>
<div class="timeline__org">STATEC-Research, Luxembourg</div>
</div>
<div class="timeline__item" markdown="1">
<span class="timeline__date">June 2019</span>
<div class="timeline__title">Inequality by the Numbers Workshop</div>
<div class="timeline__org">CUNY Graduate Center, New York</div>
</div>
</div>

## <i class="fas fa-school heading-icon"></i>Summer Schools

<div class="timeline" markdown="1">
<div class="timeline__item" markdown="1">
<span class="timeline__date">September 2022</span>
<div class="timeline__title">Causal Analysis and Machine Learning</div>
<div class="timeline__org">University of Oxford, Oxford</div>
</div>
<div class="timeline__item" markdown="1">
<span class="timeline__date">September 2019</span>
<div class="timeline__title">Explainable Data Science</div>
<div class="timeline__org">European Association for Data Science (EuADS)</div>
</div>
</div>

## <i class="fas fa-building heading-icon"></i>Research Visits

<div class="timeline" markdown="1">
<div class="timeline__item" markdown="1">
<span class="timeline__date">May - August 2019</span>
<div class="timeline__title">Visiting Researcher</div>
<div class="timeline__org">STATEC-Research, Luxembourg</div>
</div>
<div class="timeline__item" markdown="1">
<span class="timeline__date">June - August 2008</span>
<div class="timeline__title">Visiting Researcher</div>
<div class="timeline__org">Ethiopian Economics Association, Addis Ababa, Ethiopia</div>
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
