---
layout: page
title: Reading
permalink: /reading/
---

## Currently reading

_Life in Code, a personal history of technology_ by Ellen Ullman

## Archive

{% assign reading_years = site.data.reading_books | map: "year" | uniq | sort | reverse %}
{% if reading_years.size > 0 %}
<ul class="reading-years">
  {% for year in reading_years %}
    <li><a href="{{ site.baseurl }}/reading/{{ year }}/">{{ year }}</a></li>
  {% endfor %}
</ul>
{% endif %}
