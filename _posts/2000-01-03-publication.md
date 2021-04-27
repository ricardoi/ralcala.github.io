---
title: "PUBLICATION"
bg: white
color: dark
fa-icon: book
years: [2021, 2020, 2019, 2018, 2017]
---

<!-- <p>
<a href="https://scholar.google.com/citations?user=SkBxudIAAAAJ&hl=en">
  <i class="ai ai-google-scholar fa-1x"></i>
   Google Scholar
</a>
</p> -->
## -prepints and recent publications-

{% bibliography -q @unpublished %}

{% for y in page.years %}
  <h3 class="year"><font size="+3">-{{y}}-</font></h3>
  {% bibliography -q !@unpublished[year={{y}}] %}
{% endfor %}
