---
layout: page
permalink: /publications/
title: Publications
shorttitle: publications
#description: Publications by categories in reversed chronological order. Generated by jekyll-scholar.
years: [2020,2019, 2018, 2017, 2016, 2015, 2014, 2013, 2012, 2011, 2010, 2007, 2005, 2003, 2002]
---

{% for y in page.years %}
  <h3 class="year">{{y}}</h3>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
