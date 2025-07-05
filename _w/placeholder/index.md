layout: default
title: Placeholder
story: placeholder
---

{% assign chapters = site.w | where: "story", "placeholder" | sort: "chapter" %}
<ul>
  {% for chap in chapters %}
    <li><a href="{{ chap.url }}">{{ chap.title }}</a></li>
  {% endfor %}
</ul>
