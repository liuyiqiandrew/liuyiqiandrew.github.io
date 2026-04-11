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
  <a class="museum-button museum-button--outline museum-button--small" href="https://scholar.google.com/citations?user={{ site.scholar_userid }}" target="_blank" rel="noopener noreferrer">Google Scholar</a>
  <a class="museum-button museum-button--outline museum-button--small" href="https://ui.adsabs.harvard.edu/search/q=author%3A%22Liu%2C%20Yiqi%22&sort=date%20desc%2C%20bibcode%20desc&p_=0" target="_blank" rel="noopener noreferrer">NASA ADS</a>
  <a class="museum-button museum-button--outline museum-button--small" href="https://inspirehep.net/literature?sort=mostrecent&size=25&page=1&q=author%20%22Yiqi%20Liu%22" target="_blank" rel="noopener noreferrer">INSPIRE HEP</a>
</div>

<div class="publications">
  {% bibliography -f {{ site.scholar.bibliography }} -q @* %}

</div>
