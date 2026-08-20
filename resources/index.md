---
layout: default
title: Resources
description: LGBTQ+ STEM resources for oSTEM MSU members — mental health, career development, campus support, and national organizations.
---

<h1 class="page-title">Resources</h1>

A curated list of resources for LGBTQ+ students in STEM at MSU and beyond.
To suggest a resource, [contact us]({{ '/contact/' | relative_url }}) or post in the `#resources` channel on Discord.

<!-- Generated from _data/resources.yml — add new sections and links in that file -->

{% for section in site.data.resources %}
<div class="resource-section">
  <h2>{{ section.section }}</h2>
  <ul class="resource-links">
    {% for link in section.links %}
    <li>
      <a href="{{ link.url }}" target="_blank" rel="noopener noreferrer">{{ link.name }}</a>
      <span class="rl-desc">{{ link.desc }}</span>
    </li>
    {% endfor %}
  </ul>
</div>
{% endfor %}

---

*Know of a resource we should add? [Send us a suggestion.]({{ '/contact/' | relative_url }})*
