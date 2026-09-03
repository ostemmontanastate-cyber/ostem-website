---
layout: default
title: Get Involved
description: Join oSTEM MSU — attend meetings, volunteer, become a leader, and stay connected with upcoming events.
---

<h1 class="page-title">Get Involved</h1>

## Where and When We Meet

<!-- Generated automatically from _data/meetings.yml — update that file to change meeting times and location -->

{% if site.data.meetings.semester %}
**Semester:** {{ site.data.meetings.semester }}  
{% endif %}
**Regular Meetings:** {{ site.data.meetings.regular_meetings }}  
**Location:** {{ site.data.meetings.location }}  
**First meeting of each semester:** {{ site.data.meetings.first_meeting }}  

{{ site.data.meetings.notes }}

<div class="notice">
  {{ site.data.meetings.notice }}
</div>

---

## Member Availability & Interest Poll

We want to make sure our meetings, social events, and workshops work around your schedule! Please take a moment to fill out our availability and interest poll below so we can better cater our meeting times and events to when you're free, and plan activities you're excited about.

{% include poll-form.html %}

---

## Weekly Newsletter

Stay up-to-date with oSTEM MSU! Sign up for our weekly newsletter to get announcements, campus-wide event reminders, job and internship opportunities, and tips for navigating your time at MSU. You can also [open the sign-up form directly]({{ site.social.newsletter }}).

{% include newsletter-form.html %}

---

## Volunteer

Volunteering is one of the best ways to support our chapter. Beyond helping run events, **your volunteer hours directly earn funding for oSTEM MSU** through ASMSU's Volunteer & Impact Montana (VIM) program!

### Earn Funding for oSTEM Through Volunteer Hours
- **$15 per volunteer hour** — Every verified hour you log earns **$15 in funding** directly for our chapter (up to $1,500 per academic year), helping us fund meeting refreshments, community events, and conference travel.
- **What counts:** Any unpaid volunteer service completed within the State of Montana or representing MSU (e.g. community service, campus tabling, local non-profits, outreach).
- **How to log:** Track and submit your volunteer hours on **[CatServe]({{ site.social.catserve }})** and select **oSTEM at Montana State University** to receive the impact credit. You must be a member on our **CatsConnect** roster for your hours to count toward our club.

### Ways to Volunteer
- **Event setup & logistics** — Help run general meetings, social mixers, and workshops
- **Tabling & outreach** — Represent oSTEM at campus resource fairs like Catapalooza
- **Workshop facilitation** — Lead or co-lead a study night, tutorial, or professional session
- **Community & campus service** — Participate in volunteer projects across campus and Bozeman

<div class="notice">
  <strong>Need help submitting volunteer hours?</strong> Reach out to club leadership! We are here to help you get registered on CatsConnect, navigate <a href="{{ site.social.catserve }}" target="_blank" rel="noopener noreferrer">CatServe</a>, or verify your service hours. Connect with us in the <code>#volunteering</code> channel on <a href="{{ site.social.discord }}" target="_blank" rel="noopener noreferrer">Discord</a> or email an officer at <a href="mailto:{{ site.email }}">{{ site.email }}</a>.
</div>

---

## Becoming a Leadership Member

**We are actively looking for new student leaders to join our team!** Stepping into an officer role is a great way to build leadership skills, advocate for LGBTQ+ students in STEM, expand your professional network, and directly shape our chapter's events and community.

If you are interested in taking on a leadership position, please **[fill out the availability & interest poll above](#member-availability--interest-poll)**, message us in Discord, or reach out directly via email at [{{ site.email }}](mailto:{{ site.email }}).

### Open Leadership Roles & Expectations

- **Vice President** — Supports the president with chapter operations, assists with officer coordination, and helps lead general meetings and club initiatives.
- **Treasurer** — Manages chapter funds and budgets, tracks ASMSU and VIM funding allocations, and submits purchase requests on CatsConnect.
- **Secretary** — Records meeting notes and action items, maintains member records and CatsConnect rosters, and coordinates internal officer logistics.
- **Events Coordinator** — Organizes meeting agendas, coordinates social mixers and professional workshops, and arranges campus tabling events.
- **Social Media Manager** — Creates flyers and digital graphics, manages chapter social media accounts, and keeps the community engaged online.
- **Alumni / Newsletter Manager** — Curates and distributes the oSTEM Weekly newsletter, manages mailing list outreach, and maintains connections with alumni.

<div class="notice">
  <strong>Interested in leading or shadowing an officer?</strong> No previous leadership experience is required — we welcome enthusiasm, fresh ideas, and a commitment to our community. If you have questions about any position, connect with current officers on <a href="{{ site.social.discord }}" target="_blank" rel="noopener noreferrer">Discord</a> or via <a href="mailto:{{ site.email }}">{{ site.email }}</a>.
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
