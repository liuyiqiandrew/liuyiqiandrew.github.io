---
layout: page
permalink: /publications/
title: Publications
kicker: Research Output
description: Publications in cosmology and astrophysics.
nav: true
nav_order: 2
---
<!-- _pages/publications.md -->
<div class="page-shortcuts">
  <a class="museum-link-nav" href="https://scholar.google.com/citations?user={{ site.scholar_userid }}" target="_blank" rel="noopener noreferrer">Google Scholar</a>
  <a class="museum-link-nav" href="https://ui.adsabs.harvard.edu/public-libraries/GbkH5Kq6QTmSGGxvzU7YMw" target="_blank" rel="noopener noreferrer">NASA ADS</a>
  <a class="museum-link-nav" href="https://inspirehep.net/authors/2957890?ui-citation-summary=true" target="_blank" rel="noopener noreferrer">INSPIRE HEP</a>
</div>

<div class="publications">
  {% bibliography -f {{ site.scholar.bibliography }} -q @* %}

</div>
