---
layout: default
title: Get Involved
description: Join oSTEM MSU — attend meetings, volunteer, become a leader, and stay connected with upcoming events.
---

<h1 class="page-title">Get Involved</h1>

## Where and When We Meet

**Regular Meetings:** Every other Friday, 6:00 PM  
**Location:** Student Union Building, Room 212  
**First meeting of each semester:** Announced on Discord and the mailing list

Meetings are open to everyone — no RSVP needed. Just show up!

<div class="notice">
  Meeting times and rooms occasionally change. Join our <a href="{{ site.social.discord }}">Discord</a> or <a href="{{ '/contact/' | relative_url }}">mailing list</a> to get the latest updates.
</div>

---

## Volunteer

There are many ways to contribute to the chapter without holding a formal officer position:

- **Event setup and logistics** — help run general meetings and social events
- **Tabling and outreach** — represent oSTEM at campus resource fairs
- **Workshop facilitation** — lead or co-lead a professional development session
- **Conference mentorship** — help new attendees prepare for the annual conference
- **Graphic design and communications** — assist with flyers, social posts, and the website

To volunteer for a specific event or role, reach out in the `#volunteering` channel on Discord or email an officer directly.

---

## Becoming a Leadership Member

Leadership positions are elected each spring for the following academic year. All current members are eligible to run.

**Open positions typically include:**

- President
- Vice President
- Treasurer
- Secretary
- Events Coordinator
- Conference Chair

Elections are announced at the last meeting of spring semester. If you are interested in running, introduce yourself to current leadership early — shadowing an officer is a great way to prepare.

<div class="notice">
  <strong>New to the club?</strong> We strongly encourage at least one semester of general membership before running for an officer role, though it is not required.
</div>

---

## Upcoming Events

<!-- Generated from _data/events.yml — add/remove/edit events in that file -->

<div class="events-list">
{% for event in site.data.events %}
  <div class="event-item">
    <div class="event-date" aria-label="{{ event.month }} {{ event.day }}">
      <div class="ed-month">{{ event.month }}</div>
      <div class="ed-day">{{ event.day }}</div>
    </div>
    <div class="event-info">
      <div class="ei-title">{{ event.title }}</div>
      <div class="ei-meta">{{ event.time }} &mdash; {{ event.location }}</div>
      <p class="ei-desc">{{ event.description }}</p>
      {% if event.recurring %}
      <div class="ei-recurring">Recurring: {{ event.recurring }}</div>
      {% endif %}
    </div>
  </div>
{% endfor %}
</div>

*To add or update events, edit `_data/events.yml`.*
