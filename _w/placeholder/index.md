---
layout: default
title: "Placeholder — Table of Contents"
---

# Placeholder: Story Index

{% assign chapters = site.w | where: "story", "placeholder" | sort: "chapter" %}
<ol>
  {% for chap in chapters %}
    <li><a href="{{ chap.url }}">{{ chap.title }}</a></li>
  {% endfor %}
</ol>
