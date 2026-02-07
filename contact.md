---
layout: page
title: Contact
permalink: /contact/
---

<div class="contact-page">
  <h1>Contact</h1>
  
  <div class="contact-content">
    <div class="contact-info">
      <h2>Get in Touch</h2>
      <p>Interested in learning how I can help optimize your operations? Let's discuss your challenges and opportunities.</p>
      
      <div class="contact-details">
        <div class="contact-item">
          <h3>Location</h3>
          <p>{{ site.author.location }}</p>
        </div>
        
        <div class="contact-item">
          <h3>Email</h3>
          <p><a href="mailto:{{ site.author.email }}">{{ site.author.email }}</a></p>
        </div>
        
        <div class="contact-item">
          <h3>Phone</h3>
          <p><a href="tel:{{ site.author.phone }}">{{ site.author.phone }}</a></p>
        </div>
        
        <div class="contact-item">
          <h3>LinkedIn</h3>
          <p><a href="{{ site.author.linkedin }}" target="_blank" rel="noopener">Connect on LinkedIn</a></p>
        </div>
      </div>
    </div>
    
    <div class="contact-form-section">
      <h2>Send a Message</h2>
      <p class="form-note">Note: You'll need to add a form service like Formspree or use a contact form plugin. For now, visitors can use the email/phone above.</p>
      
      <!-- Optional: Add Formspree or similar service -->
      <!-- 
      <form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
        <div class="form-group">
          <label for="name">Name</label>
          <input type="text" id="name" name="name" required>
        </div>
        
        <div class="form-group">
          <label for="email">Email</label>
          <input type="email" id="email" name="_replyto" required>
        </div>
        
        <div class="form-group">
          <label for="message">Message</label>
          <textarea id="message" name="message" rows="5" required></textarea>
        </div>
        
        <button type="submit" class="btn btn-primary">Send Message</button>
      </form>
      -->
    </div>
  </div>
</div>
