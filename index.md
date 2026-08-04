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

<!-- MAIN CENTERED COLUMN WRAPPER -->
<div class="page-container">

  <section class="section-card">
    <h2>Welcome to Ramsbury & District MRC!</h2>
    <p>Welcome to Ramsbury and District Model Railway Club. We are a friendly bunch who meet every Tuesday evening and Saturday morning in Ramsbury, North East Wiltshire. We currently have projects in both N and 00 gauge as well as a fully operational sound-fitted exhibition layout.</p>
  </section>

  <section class="section-card">
    <h3>When and Where We Meet</h3>
    <p>We meet every Tuesday 18:30 - 21:00 and Saturday 09:00 - 13:00.</p>
    <p>Fox & Hounds Dairy, Crowood Ln, Ramsbury, Wilts, SN8 2HE</p>
  </section>

  <!-- Centered Map Container inside the column -->
  <div class="map-container">
    <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d9944.883104670163!2d-1.6050327747172464!3d51.45410282477082!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x487153100a74abb3%3A0xabef1753274a7d0b!2sRamsbury%20and%20District%20Model%20Railway%20Club!5e0!3m2!1sen!2suk!4v1785877718525!5m2!1sen!2suk" width="600" height="350" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="strict-origin-when-cross-origin"></iframe>
  </div>

  <section class="section-card" id="contact">
    <h3>Contact</h3>
    <ul>
      <li><strong>Phone:</strong> 12345 67890</li>
      <li><strong>Email:</strong> test@email.com</li>
    </ul>
  </section>

</div> <!-- END OF PAGE CONTAINER -->

<!-- Stylesheet -->
<style>
  /* Define your variables here! Change these to tweak the whole site instantly */
  :root {
    --light-stone: #B88359;
    --dark-stone: #936D58;
    --bevel: 8px; /* Change this number to adjust all rounded corners at once */
  }

  /* Outer screen background uses Dark Stone */
  html, body {
    background-color: var(--dark-stone) !important; 
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
    color: #333333;
    line-height: 1.6;
    margin: 0;
    padding: 20px;
    height: 100%;
  }

  /* Header area - Now uses uniform bevel */
  .mrc-header {
    max-width: 600px;
    margin: 0 auto 20px auto;
    display: flex;
    align-items: center;
    justify-content: space-between;
    flex-wrap: wrap;
    background-color: var(--light-stone) !important; 
    padding: 12px 18px;
    border-radius: var(--bevel); 
  }

  /* Inner column wrapper - Now uses uniform bevel */
  .page-container {
    max-width: 600px;
    margin: 0 auto;
    display: flex;
    flex-direction: column;
    gap: 20px;
    background-color: var(--light-stone) !important; 
    padding: 25px;
    border-radius: var(--bevel);       
  }

  /* Individual content cards - Transparent so they show the Light Stone */
  .section-card {
    background: transparent !important; 
    padding: 0;              
  }

  img {
    max-width: 100%;
    height: auto;
  }

  /* Logo explicitly stripped of bevels */
  .mrc-logo {
    max-height: 100px;
    width: auto;
    border-radius: 0 !important; /* Forces the logo to remain perfectly square */
  }

  .mrc-button-row {
    display: flex;
    gap: 10px;
  }

  /* Button Styling - Now uses uniform bevel */
  .mrc-btn {
    background-color: var(--dark-stone); /* Fixed var() syntax */
    color: #ffffff !important;
    padding: 8px 14px;
    text-decoration: none;
    border-radius: var(--bevel); 
    font-weight: bold;
    font-size: 14px;
    transition: background-color 0.2s ease, filter 0.2s ease;
  }

  /* Fixed hover state so it actually changes color (slightly darker) */
  .mrc-btn:hover {
    background-color: var(--dark-stone);
    filter: brightness(0.85); /* Makes the stone color 15% darker on hover */
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

  /* The small lines of the hamburger menu don't use the large uniform bevel */
  .hamburger-icon span {
    display: block;
    height: 3px;
    width: 100%;
    background-color: #2c3e50;
    border-radius: 3px; 
  }

  /* Map Container */
  .map-container {
    width: 100%;
    background: transparent !important;
    display: flex;
    justify-content: center;
    box-sizing: border-box;
  }

  /* Map Iframe - Now uses uniform bevel */
  .map-container iframe {
    width: 100%;
    max-width: 100%;
    height: 350px;
    border-radius: var(--bevel);
    display: block;
  }

  /* Mobile Responsive Breakpoint */
  @media (max-width: 768px) {
    html, body {
      padding: 10px;
    }

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