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
      <!-- Replace with real email -->
      <a href="mailto:ostem@msu.example.edu">ostem.montanastate@gmail.com</a>
    </p>

    <h3>Discord</h3>
    <p>
      The fastest way to reach us. Join our server and post in
      <code>#general</code> or DM an officer.<br>
      <a href="https://discord.gg/jhkHnVwd6e" target="_blank" rel="noopener noreferrer">Join our Discord →</a>
    </p>

    <h3>Linktree</h3>
    <p>
      All our links in one place — social media, newsletter signup, and more.<br>
      <a href="https://linktr.ee/ostem.msu" target="_blank" rel="noopener noreferrer">https://linktr.ee/ostem.msu →</a>
    </p>

    <h3>Campus Address</h3>
    <p>
      <!-- Update with real location if applicable -->
      Montana State University<br>
      Bozeman, MT 59717
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
