---
layout: page
title: Reading
permalink: /reading/
---

I started loosely tracking my reading in 2019.
I don't take notes and I don't rate books.
The only review I've ever done publicly is <a href="{{ site.baseurl }}/thirty/">30 for 30</a>.

## Currently reading

The Master & Margarita - Mikhail Bulgakov

Ethics in the Real World - Peter Singer

## Bookshelf

{% assign reading_years = site.data.reading_books | map: "year" | uniq | sort | reverse %}
{% if reading_years.size > 0 %}
<ul class="reading-years">
  {% for year in reading_years %}
    <li><a href="{{ site.baseurl }}/reading/{{ year }}/">{{ year }}</a></li>
  {% endfor %}
</ul>
{% endif %}
