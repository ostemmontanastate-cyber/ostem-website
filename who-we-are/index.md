---
layout: default
title: Who We Are
description: Learn about oSTEM at Montana State University — our history, mission, and current leadership team.
---

<h1 class="page-title">Who We Are</h1>

## Our Mission

oSTEM at Montana State University is a chapter of oSTEM Inc., a national non-profit organization supporting LGBTQ+ students pursuing careers in STEM. We provide a space for community building, professional development, and advocacy — creating a more inclusive future for science and engineering at MSU and beyond.

## History

<!-- Update this section with your chapter's founding story. -->

oSTEM MSU was founded in **2016** by a small group of LGBTQ+ students in the College of Engineering and the College of Letters & Science who recognized the need for a dedicated community on campus.

Since then, the chapter has grown steadily. What began as informal study groups and social meetups has expanded into a full calendar of events including professional development workshops, the annual oSTEM Conference trip, and ongoing advocacy for LGBTQ+-inclusive policies at MSU.

Today, the chapter connects students across all STEM disciplines — from computer science to biology, from chemistry to civil engineering — and collaborates with campus partners including the Spectrum Center and the Office of Diversity & Inclusion.

## Where We Are Today

- **Active, student-led** with regular elected leadership
- **Participating in the annual oSTEM National Conference** each fall
- **Partnering with MSU departments and offices** to improve inclusion in STEM programs
- **Open to all students** — you do not need to identify as LGBTQ+ to participate

<div class="notice">
  <strong>Leadership rotates frequently.</strong> If you are looking to collaborate with our chapter — for events, sponsorships, or partnerships — we recommend reaching out via email or Discord to ensure you're in contact with current officers. See <a href="{{ '/contact/' | relative_url }}">Contact Us</a>.
</div>

## Current Leadership

<!-- This section is generated automatically from _data/leadership.yml -->
<!-- To update: edit _data/leadership.yml with current names, roles, and pronouns -->

<div class="leadership-grid">
{% for person in site.data.leadership %}
  <div class="leadership-card">
    <div class="lc-role">{{ person.role }}</div>
    <div class="lc-name">{{ person.name }}</div>
    {% if person.pronouns %}
    <div class="lc-pronouns">{{ person.pronouns }}</div>
    {% endif %}
    {% if person.email %}
    <a class="lc-email" href="mailto:{{ person.email }}">{{ person.email }}</a>
    {% endif %}
  </div>
{% endfor %}
</div>

*Leadership is elected each academic year. Positions and officers are subject to change.*
