---
layout: page
title: About
permalink: /about/
---


Free, open source 3D Slicer extension for image-based 3D motion tracking of skeletal structures

Integrating advanced videoradiography, 4DCT registration, and hierarchical 3D registration for cutting-edge biomechanical research

<style>
  .resource-grid {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    gap: 1.5rem;
    justify-content: space-around;
    margin-top: 2rem;
  }

  .resource-card {
    border: 1px solid #e0e0e0;
    border-radius: 8px;
    padding: 1rem;
    text-align: center;
    background-color: #fafafa;
    box-shadow: 0 2px 4px rgba(0,0,0,0.05);
  }

  .resource-card i {
    font-size: 2rem;
    margin-bottom: 0.5rem;
    color: #333;
  }
</style>

<div class="resource-grid">
  <div class="resource-card">
    <i class="fas fa-comments"></i>
    <h4>Discourse</h4>
    <p>Join the community and get answers to your questions.</p>
    <p>
      <a href="https://discourse.slicer.org/c/community/slicerautoscoperm/30" target="_blank">
        Visit Forum →
      </a>
    </p>
  </div>

  <div class="resource-card">
    <i class="fab fa-github"></i>
    <h4>GitHub Repository</h4>
    <p>Access source code, report issues, and contribute to development.</p>
    <p>
      <a href="https://github.com/BrownBiomechanics" target="_blank">
        Go to GitHub →
      </a>
    </p>
  </div>

  <div class="resource-card">
    <i class="fas fa-book-open"></i>
    <h4>Documentation</h4>
    <p>Comprehensive guides, tutorials, and API documentation.</p>
    <p>
      <a href="https://autoscoper.readthedocs.io/" target="_blank">
        Read Docs →
      </a>
    </p>
  </div>
</div>

<br/>

* [Team]({% link team.md %})
* [License](https://autoscoper.readthedocs.io/en/latest/about.html#license)
* [How to cite](https://autoscoper.readthedocs.io/en/latest/about.html#how-to-cite)
* [Acknowledgments]({% link acknowledgments.md %})
* [Call for Collaboration]({% link call-for-collaboration.md %})

<br/>

## Contact the Team

If you prefer to reach out privately instead of posting in the public
Discourse forum, you can use the form below to contact the team directly.

<form action="https://docs.google.com/forms/d/e/1FAIpQLSdV3YkJQg0aJ3utMx_Qh10iVJtTcyyznQctZWB7Kf6wHjRHpA/formResponse" method="POST" class="contact-form">
  <div class="form-row">
    <div class="form-field">
      <label for="first-name">First Name</label>
      <input type="text" id="entry.1180021443" name="first-name" required />
    </div>
    <div class="form-field">
      <label for="last-name">Last Name</label>
      <input type="text" id="entry.254693434" name="last-name" required />
    </div>
  </div>

  <div class="form-group">
    <label for="email">Email</label>
    <input type="email" id="entry.1416781666" name="email" required
           pattern="[a-zA-Z0-9_\.\+-]+@[a-zA-Z0-9-]+\.[a-zA-Z0-9-\.]+"
           title="Please enter a valid email address." />
  </div>

  <div class="form-group">
    <label for="message">Message</label>
    <textarea id="entry.2084414223" name="message" rows="6" required></textarea>
  </div>

  <div class="form-group">
    <button type="submit">Send Message</button>
  </div>
</form>

<style>
  .contact-form {
    max-width: 600px;
    margin-top: 1rem;
  }

  .form-row {
    display: flex;
    flex-wrap: wrap;
    gap: 1rem;
  }

  .form-field {
    flex: 1 1 45%;
  }

  .form-group, .form-field {
    margin-top: 1rem;
  }

  .contact-form label {
    display: block;
    font-weight: bold;
    margin-bottom: 0.25rem;
  }

  .contact-form input,
  .contact-form textarea {
    width: 100%;
    padding: 0.5rem;
    border: 1px solid #ccc;
    border-radius: 4px;
    font: inherit;
  }

  .contact-form button {
    padding: 0.6rem 1.2rem;
    background-color: #007acc;
    color: white;
    border: none;
    border-radius: 4px;
    cursor: pointer;
  }

  .contact-form button:hover {
    background-color: #005ea8;
  }
</style>
