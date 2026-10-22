---
title: ""
layout: archive
sitemap: true
permalink: /
author_profile: true
classes: wide
---

<div class="eyebrow"> Data Science &middot; Economics &middot; AI &middot; Privacy</div>
<h1 class="headline">Connecting data science, research and responsible data reuse.</h1>
<p class="lead">I help public and private partners create value from data. My work focuses on responsible data reuse, privacy-enhancing technologies, data service design and delivery, and data projects from scoping to implementation. I also deliver training.</p>

<div class="btn-row" markdown="1">
[View CV](/cv/){: .btn .btn--primary}
[View Research &rarr;](/research/){: .btn .btn--outline}
</div>

## Research Focus

I develop explainable machine learning and applied microeconometric methods to study poverty, inequality, labour markets, and health economics.

My methodological interests span interpretable and causal machine learning, and quasi-experimental methods. I also have a growing research interest in privacy-preserving data science, particularly methods that enable rigorous analysis while safeguarding individual privacy.

My applied research focuses on development, health, and household economics, including well-being, material and social deprivation, vulnerability to poverty, and protective behaviours during health crises.

## Research Focus

I develop explainable machine learning and applied microeconometric methods to study poverty, inequality, labour markets, and health economics.

My methodological interests span interpretable and causal machine learning, and quasi-experimental methods. I also have a growing research interest in privacy-preserving data science, particularly methods that enable rigorous analysis while safeguarding individual privacy.

My applied research focuses on development, health, and household economics, including well-being, material and social deprivation, vulnerability to poverty, and protective behaviours during health crises.

<div class="divider"><span>&#9670;</span></div>

## Selected Research

<!-- Pulled from _data/publications.yml (entries with featured: true) so this
     section can never drift out of sync with /research/ - edit a paper's
     status/citation/etc. there and it updates here automatically.
     Optional: add "image: /assets/images/your-figure.png" to a featured entry
     to show its figure above the text. The figure links to the paper's entry
     on /research/. Entries without an image display exactly as before. -->
<div class="cards" markdown="1">
{% for pub in site.data.publications %}{% if pub.featured %}
<div class="card" markdown="1">
{% if pub.image %}<a href="/research/#{{ pub.id }}"><img src="{{ pub.image | relative_url }}" alt="Key figure from: {{ pub.title | escape }}" loading="lazy" style="width:100%;height:auto;border-radius:6px;margin-bottom:0.75rem;"></a>{% endif %}

<span class="card__tag">{{ pub.venue }}</span>

**{{ pub.title }}**

{{ pub.blurb }}

[Read more &rarr;](/research/#{{ pub.id }}){: .inline-link}
</div>
{% endif %}{% endfor %}
</div>

## Recent Blogs

<div class="card" markdown="1">
_New posts coming soon._ In the meantime, check out [a few quotes I like](/misc/).
</div>

## Recent & Upcoming Talks

<!-- Pulled from _data/talks.yml. Add one entry per talk there; this section
     updates automatically. Until the file has entries, a short note shows. -->
<div class="card" markdown="1">
{% if site.data.talks and site.data.talks.size > 0 %}{% for talk in site.data.talks %}
**{{ talk.title }}**

{{ talk.event }}{% if talk.location %}, {{ talk.location }}{% endif %} &middot; {{ talk.date }}{% if talk.slides %} &middot; [Slides]({{ talk.slides }}){% endif %}
{% endfor %}{% else %}
_Talks and presentations will be listed here soon._
{% endif %}
</div>

***
<!-- Moved out of the home page to avoid repeating the CV and sidebar. Suggested homes:
Removed hero title: "Machine learning meets applied microeconomics".
CV page: doctoral researcher in the DRIVEN research team (Department of Economics and Management, University of Luxembourg); earlier role as Assistant Research Officer, Economic Modeling and Statistical Analysis Department, Central Bank of Ethiopia.
Misc page: outside of research, painting and photography; giving back to the community.
Old intro line removed: "currently on the job market".

, and I have volunteered with [insert the organizations with which you have volunteered].
<i class='fas fa-download' style='font-size:18px'></i> You can download my full <a target="_blank" href="/_pages/Taye_cv.pdf">Curriculum Vitae <i class="far fa-file-pdf"></i></a> here.
-->