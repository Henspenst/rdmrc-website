---
title: Home
layout: default
---

<!-- Navigation & Header Bar -->
<div class="mrc-header">
  <img src="images/logo.jpg" alt="MRC Logo" class="mrc-logo">

  <!-- Hidden checkbox for mobile toggle -->
  <input type="checkbox" id="menu-toggle" class="menu-checkbox">
  
  <!-- Hamburger Icon -->
  <label for="menu-toggle" class="hamburger-icon">
    <span></span>
    <span></span>
    <span></span>
  </label>

  <!-- Button Links -->
  <div class="mrc-button-row">
    <a href="index.md" class="mrc-btn">Home</a>
    <a href="layouts.md" class="mrc-btn">Layouts</a>
    <a href="events.md" class="mrc-btn">Events</a>
    <a href="contact.md" class="mrc-btn">Contact</a>
  </div>
</div>

<section class="section-card">
  <h2>Welcome to Ramsbury & District MRC!</h2>
  <p>Welcome to Ramsbury and District Model Railway Club. We are a friendly bunch who meet every Tuesday evening and Saturday morning in Ramsbury, north east Wiltshire. We currently have projects in both N and 00 gauge as well as a fully operational sound-fitted exhibition layout.</p>
</section>

<div class="section-grid">
  <section class="section-card">
    <h3>When and Where We Meet</h3>
    <p>We meet every Tuesday 18:30 - 21:00 and Saturday 09:00 - 13:00.</p>
    <p>Fox & Hounds Dairy, Crowood Ln, Ramsbury, Wilts, SN8 2HE</p>
  </section>
  <div class="map-container">
    <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d9944.883104670163!2d-1.6050327747172464!3d51.45410282477082!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x487153100a74abb3%3A0xabef1753274a7d0b!2sRamsbury%20and%20District%20Model%20Railway%20Club!5e0!3m2!1sen!2suk!4v1785877718525!5m2!1sen!2suk" width="350" height="350" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="strict-origin-when-cross-origin"></iframe>
  </div>
</div>

<section class="section-card" id="contact">
  <h3>Contact</h3>
  <p>If you want to add a contact section, use a simple Markdown block or a custom HTML snippet in this page. Keep the design consistent with the classic railway theme by using green and gold accents.</p>
  
  <!-- Map wrapped in its container -->
  
</section>

<!-- Combined Stylesheet for Navigation, Responsiveness, and General Layout -->
<style>
  /* Global image safety */
  img {
    max-width: 100%;
    height: auto;
    border-radius: 8px;
  }

  /* Header & Navigation Layout */
  .mrc-header {
    display: flex;
    align-items: center;
    justify-content: space-between;
    flex-wrap: wrap;
    background: #f8f9fa;
    padding: 12px 18px;
    border-radius: 8px;
    margin-bottom: 25px;
    box-shadow: 0 2px 5px rgba(0,0,0,0.05);
  }

  .mrc-logo {
    max-height: 100px;
    width: auto;
  }

  .mrc-button-row {
    display: flex;
    gap: 10px;
  }

  /* Button Styling (Railway Theme Ready) */
  .mrc-btn {
    background-color: #2c3e50;
    color: #ffffff !important;
    padding: 8px 14px;
    text-decoration: none;
    border-radius: 5px;
    font-weight: bold;
    font-size: 14px;
    transition: background-color 0.2s ease;
  }

  .mrc-btn:hover {
    background-color: #1abc9c;
  }

  /* Hidden Checkbox for Mobile Toggle */
  .menu-checkbox {
    display: none;
  }

  /* Hamburger Icon Base Styles */
  .hamburger-icon {
    display: none;
    flex-direction: column;
    justify-content: space-between;
    width: 30px;
    height: 21px;
    cursor: pointer;
  }

  .hamburger-icon span {
    display: block;
    height: 3px;
    width: 100%;
    background-color: #2c3e50;
    border-radius: 3px;
  }

  /* Map Container & Responsive Styling */
  .map-container {
    width: 100%;
    margin-top: 15px;
    border-radius: 8px;
    overflow: hidden;
    box-shadow: 0 2px 5px rgba(0,0,0,0.1);
    line-height: 0; /* Prevents inline spacing bugs under the iframe */
  }

  .map-container iframe {
    width: 100%;
    height: 350px; /* Forces height explicitly */
    display: block;
  }

  /* Mobile Responsive Breakpoint (Screens under 768px) */
  @media (max-width: 768px) {
    .hamburger-icon {
      display: flex;
    }

    .mrc-button-row {
      display: none;
      width: 100%;
      flex-direction: column;
      gap: 8px;
      margin-top: 15px;
    }

    .menu-checkbox:checked ~ .mrc-button-row {
      display: flex;
    }
  }
</style>