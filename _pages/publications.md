---
layout: page
permalink: /publications/
title: publications
description: publications in reverse chronological order.
nav: true
nav_order: 2
---

{% include bib_search.liquid %}

<p class="small">
{% for convention_pair in site.data.authorship %}
  {% assign convention = convention_pair[1] %}
  <sup>{{ convention.symbol }}</sup> {{ convention.description }}{% unless forloop.last %}; {% endunless %}
{% endfor %}
</p>

<div class="publications">

{% bibliography %}

</div>
