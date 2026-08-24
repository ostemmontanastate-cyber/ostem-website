---
layout: default
title: Contact Us
description: Get in touch with oSTEM at Montana State University — email, Discord, and general contact form.
---

<h1 class="page-title">Contact Us</h1>

<div class="contact-grid">

  <div class="contact-info">
    <h2 style="margin-top:0;">Reach Out</h2>
    <p>
      Have a question, want to collaborate, or just want to say hello?
      Use the form or contact an officer directly.
    </p>

    <h3>General Inquiries</h3>
    <p>
      <a href="mailto:{{ site.email }}">{{ site.email }}</a>
    </p>

    <h3>Discord</h3>
    <p>
      The fastest way to reach us. Join our server and post in
      <code>#general</code> or DM an officer.<br>
      <a href="{{ site.social.discord }}" target="_blank" rel="noopener noreferrer">Join our Discord →</a>
    </p>

    <h3>Linktree</h3>
    <p>
      All our links in one place — social media, discord, and more.<br>
      <a href="{{ site.social.linktree }}" target="_blank" rel="noopener noreferrer">{{ site.social.linktree }} →</a>
    </p>

    <h3>Weekly Newsletter</h3>
    <p>
      Sign up for weekly chapter updates, campus events, and opportunities.<br>
      <a href="{{ site.social.newsletter }}" target="_blank" rel="noopener noreferrer">Subscribe to our newsletter →</a>
    </p>

  </div>

  <div class="contact-form-col">
    <h2 style="margin-top:0;">Send a Message</h2>
    <form class="application-form" id="contact-form"
          action="https://formspree.io/f/xjyblrjb"
          method="POST">

      <div class="form-group">
        <label for="contact-name">Your Name *</label>
        <input type="text" id="contact-name" name="name" required placeholder="Full name">
      </div>

      <div class="form-group">
        <label for="contact-email">Your Email *</label>
        <input type="email" id="contact-email" name="email" required placeholder="you@example.com">
      </div>

      <div class="form-group">
        <label for="contact-subject">Subject</label>
        <input type="text" id="contact-subject" name="subject" placeholder="What's this about?">
      </div>

      <div class="form-group">
        <label for="contact-message">Message *</label>
        <textarea id="contact-message" name="message" required
                  placeholder="Your message here…"></textarea>
      </div>

      <button type="submit" class="btn" id="contact-submit">Send Message</button>
    </form>
  </div>

</div>

---

<div class="notice">
  <strong>For partnerships, sponsorships, or department inquiries</strong> — please email us directly
  and include your organization name and the nature of the request. We respond within a few business days.
</div>
