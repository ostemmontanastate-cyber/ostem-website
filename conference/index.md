---
layout: default
title: oSTEM Conference
description: Learn about the annual oSTEM National Conference and how MSU chapter members can apply for funding to attend.
---

<h1 class="page-title">oSTEM Conference</h1>

## Why Attend?

The **oSTEM Annual Conference** is the world's largest gathering of LGBTQ+ people in STEM. Held every fall, it brings together thousands of students, professionals, and employers for three days of networking, career development, and community.

- Connect with LGBTQ+-friendly employers from Fortune 500 companies to national labs
- Attend workshops on professional skills, research, and leadership
- Meet oSTEM chapter members from across the country
- Participate in the career fair — many attendees receive internship and full-time offers

**When:** Every fall (typically late October – early November)  
**Who can apply:** All MSU oSTEM members  
**What's covered:** Airfare, shared lodging, group meals, and conference registration — fully funded for selected attendees

---

## Preferred Requirements for Attendance

To be considered for fully funded conference attendance, applicants are expected to show active involvement and dedication to the MSU oSTEM community through one (or a mix) of the following pathways:

- **Holding or stepping into an active leadership role** within the chapter
- **Registering at least 20 VIM volunteer hours** credited to oSTEM on [CatServe]({{ site.social.catserve }})
- **Attending at least 70% of general meetings and chapter events** throughout the year
- **A combination or mix of the above suggestions** — *Example:* If you aren't able to make it to every meeting due to class conflicts, but you volunteered 10 hours and helped an officer with several weekly emails, event setup, or tabling, that counts toward your eligibility!

### Maximize Your Chances: Connect with Leadership
We strongly encourage members to reach out directly to current leadership early on! You can consult and negotiate flexible arrangements on effort, tasks, or projects you can take on to assist the club and strengthen your chances of being selected for the conference. Reach out in the `#conference` channel on [Discord]({{ site.social.discord }}) or email us at [{{ site.email }}](mailto:{{ site.email }}).

<div class="notice">
  <strong>Why these requirements?</strong> Fully-funded conference travel is a massive perk of club membership made possible through university funding and donor support. Our goal is to ensure that conference attendees are dedicated maintainers and retainers of oSTEM MSU who will bring their knowledge, enthusiasm, and leadership back to sustain and grow our campus community. Giving back to the chapter is heavily encouraged!
</div>

---

{% assign current = site.data.conferences | first %}

## {{ current.year }} oSTEM Conference

{{ current.description }}

**Dates:** {{ current.dates }}  
**Location:** {{ current.location }}  
**Capacity:** Up to {{ current.capacity }} students supported  
**Application deadline:** {{ current.application_deadline }}

{% if current.participants %}
### Selected Participants

The following students were selected from the early application deadline. Additional students will be selected from the main deadline.

<ul class="participant-list">
{% for name in current.participants %}
  <li>{{ name }}</li>
{% endfor %}
</ul>
{% endif %}

{% if current.hotel_rooms %}
### Hotel — {{ current.hotel }}

<table class="itinerary-table">
{% for room in current.hotel_rooms %}
  <tr><td><strong>{{ room.label }}</strong></td><td>{{ room.occupants }}</td></tr>
{% endfor %}
</table>
{% endif %}

{% if current.itinerary %}
### Travel Itinerary

<div class="itinerary-list">
{% for block in current.itinerary %}
  <div class="itinerary-day">
    <div class="itin-day-label">{{ block.day }}</div>
    <ul class="itin-events">
    {% for ev in block.events %}
      <li>{{ ev }}</li>
    {% endfor %}
    </ul>
  </div>
{% endfor %}
</div>
{% endif %}

---

## Apply — Due {{ current.application_deadline }} {#apply}

<form class="application-form" id="conference-application-form"
      action="https://formspree.io/f/xgawdyqn"
      method="POST">

  <div class="form-group">
    <label for="conf-name">Full Legal Name *</label>
    <input type="text" id="conf-name" name="name" required placeholder="As it appears on your government ID">
  </div>

  <div class="form-group">
    <label for="conf-dob">Date of Birth *</label>
    <input type="date" id="conf-dob" name="date_of_birth" required>
    <span class="form-note">Used for airline ticket purchase if selected.</span>
  </div>

  <div class="form-group">
    <label for="conf-gender">Gender (for ID/ticketing purposes) *</label>
    <input type="text" id="conf-gender" name="gender" required placeholder="As it appears on your government ID">
  </div>

  <div class="form-group">
    <label for="conf-email">MSU Email *</label>
    <input type="email" id="conf-email" name="email" required placeholder="netid@montana.edu">
  </div>

  <div class="form-group">
    <label for="conf-major">Major / Program *</label>
    <input type="text" id="conf-major" name="major" required placeholder="e.g. Computer Science, Biology">
  </div>

  <div class="form-group">
    <label for="conf-year">Year in School *</label>
    <select id="conf-year" name="year" required>
      <option value="">Select one…</option>
      <option>First Year</option>
      <option>Sophomore</option>
      <option>Junior</option>
      <option>Senior</option>
      <option>Graduate Student</option>
    </select>
  </div>

  <div class="form-group">
    <label for="conf-involvement">Anticipated future involvement with oSTEM MSU *</label>
    <textarea id="conf-involvement" name="future_involvement" required
      placeholder="Describe how you plan to stay involved with oSTEM after attending the conference. You may also mention past involvement with oSTEM or similar clubs…"></textarea>
  </div>

  <div class="form-group">
    <label for="conf-why">Why you would like to attend the conference *</label>
    <textarea id="conf-why" name="why_attend" required
      placeholder="Tell us what you hope to get out of the experience…"></textarea>
  </div>

  <div class="form-group">
    <label for="conf-notes">Anything else you would like to add (optional)</label>
    <textarea id="conf-notes" name="additional_notes"
      placeholder="Dietary restrictions, accessibility needs, questions, etc."></textarea>
  </div>

  <div class="form-group">
    <label for="conf-resume">Resume (PDF) *</label>
    <input type="file" id="conf-resume" name="resume" accept=".pdf">
    <span class="form-note">Attach your current resume as a PDF.</span>
  </div>

  <button type="submit" class="btn" id="conf-submit">Submit Application</button>
  <p class="form-note" style="margin-top:0.75rem;">
    Questions? Email <a href="mailto:{{ current.faculty_email }}">{{ current.faculty_advisor }}</a>.
  </p>
</form>

---

## Past Conferences

{% for conf in site.data.conferences offset: 1 %}
<div class="conference-entry">
  <div class="ce-year">{{ conf.year }}</div>
  <div class="ce-body">
    <div class="ce-location">{{ conf.location }}</div>
    <div class="ce-dates">{{ conf.dates }}</div>
    <p class="ce-desc">{{ conf.description }}</p>
    <div class="ce-attendees">{{ conf.attendees }} MSU attendee{% if conf.attendees != 1 %}s{% endif %}</div>

    {% comment %}
      Photo gallery — drops images from assets/conference-photos/PHOTO_FOLDER/
      Add photos by dropping .jpg/.jpeg/.png/.webp files into the matching subfolder.
      They appear here automatically after the next Jekyll build.
    {% endcomment %}
    {% assign folder = conf.photo_folder %}
    {% if folder %}
    <div class="photo-gallery" id="gallery-{{ conf.year }}">
      {% for file in site.static_files %}
        {% if file.path contains folder %}
          {% if file.extname == '.jpg' or file.extname == '.jpeg' or file.extname == '.png' or file.extname == '.webp' or file.extname == '.JPG' or file.extname == '.JPEG' or file.extname == '.PNG' or file.extname == '.WEBP' %}
      <a class="photo-thumb"
         href="{{ file.path | relative_url }}"
         target="_blank"
         rel="noopener"
         aria-label="{{ conf.year }} conference photo">
        <img src="{{ file.path | relative_url }}"
             alt="{{ conf.year }} oSTEM Conference — {{ conf.location }}"
             loading="lazy">
      </a>
          {% endif %}
        {% endif %}
      {% endfor %}
    </div>
    {% endif %}
  </div>
</div>
{% endfor %}

<div class="notice" style="margin-top:1.5rem;">
  <strong>Have photos?</strong> Drop them into <code>assets/conference-photos/conference-YEAR/</code>
  and they will appear here automatically after the next site build. Supported formats: JPG, PNG, WebP.
</div>
