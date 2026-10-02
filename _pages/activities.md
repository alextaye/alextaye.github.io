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

## Selected Conferences & Workshops

* IARIW 37th General Conference, Luxembourg, August 2022. <br>
* Well-Being 2022 Conference, STATEC, Luxembourg, June 2022. <br>
* The 14th Workshop on Labour Economics–IAAEU, University of Trier, April 2022. <br>
* Brownbag Seminar, STATEC-Research, Luxembourg, April 2022. <br>
* Inequality by the Numbers workshop, CUNY Graduate Center, New York, Jun 2019. <br>

## Summer Schools

* Causal Analysis and Machine Learning, University of Oxford, Oxford, September 2022. <br>
* Explainable Data Science, European Association for Data Science (EuADS), September 2019.

## Research Visits

* STATEC-Research, Luxembourg, May - August 2019.<br>
* Ethiopian Economics Association, Addis Ababa, Ethiopia, Jun - August 2008.

## <i class="fas fa-globe-africa heading-icon"></i>Places I have been

{% include visited-map.html %}

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
