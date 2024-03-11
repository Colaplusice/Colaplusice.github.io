---
layout: page
permalink: /publications/
title: publications
description: I attempt to keep this list up to date. Also check my <a href="https://scholar.google.com/citations?user=6LAGBq8AAAAJ">Google Scholar</a> profile.
years: [2022,2021]
journals: [2022]
conferences: [2021]
---
{% for y in page.years %}
  <h3 class="year">{{y}}</h3>
  {% if page.journals contains y %}
  <strong>Journal Articles</strong>
  {% bibliography -f journals -q @*[year={{y}}]* %}
  {% endif %}
  {% if page.conferences contains y %}
  <strong>Conference Publications</strong>
  {% bibliography -f conferences -q @*[year={{y}}]* %}
  {% endif %}
{% endfor %}
