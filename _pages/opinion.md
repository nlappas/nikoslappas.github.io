---
layout: page
permalink: /opinion/
title: opinion
description: This page includes a series of personal takes on several issues ranging from public policy to sports...
---

<ul class="post-list">
{% for opinion in site.opinion reversed %}
    <li>
        <h2><a class="poem-title" href="{{ opinion.url | prepend: site.baseurl }}">{{ opinion.title }}</a></h2>
        <p class="post-meta">{{ opinion.date | date: "%B %-d, %Y" }}</p>
      </li>
{% endfor %}
</ul>
