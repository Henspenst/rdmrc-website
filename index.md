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
  body {
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
    color: #333333;
    line-height: 1.6;
    background-color: #f0f2f5; /* Optional: Soft background color to make the column pop */
    margin: 0;
    padding: 20px;
  }

  /* Central Column Wrapper */
  .page-container {
    max-width: 600px; /* Controls how wide the column is */
    margin: 0 auto;    /* Centers the column horizontally */
    display: flex;
    flex-direction: column;
    gap: 20px;         /* Adds clean spacing between sections */
    background: #fffbd0;
  }

  /* Style for individual content cards */
  .section-card {
    padding: 25px;
    border-radius: 8px;
    box-shadow: 0 2px 5px rgba(0,0,0,0.05);
  }

  img {
    max-width: 100%;
    height: auto;
    border-radius: 8px;
  }

  /* Header & Navigation Layout */
  .mrc-header {
    max-width: 800px;
    margin: 0 auto 20px auto; /* Matches the page container width and centers it */
    display: flex;
    align-items: center;
    justify-content: space-between;
    flex-wrap: wrap;
    background: #ffffff;
    padding: 12px 18px;
    border-radius: 8px;
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

  /* Button Styling */
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

  /* Centered Map Container */
  .map-container {
    width: 100%;
    background: #ffffff;
    padding: 15px;
    border-radius: 8px;
    display: flex;
    justify-content: center;
    box-shadow: 0 2px 5px rgba(0,0,0,0.05);
    box-sizing: border-box;
  }

  .map-container iframe {
    width: 100%;
    max-width: 100%;
    height: 350px;
    border-radius: 6px;
    display: block;
  }

  /* Mobile Responsive Breakpoint (Screens under 768px) */
  @media (max-width: 768px) {
    body {
      padding: 10px; /* Reduces outer padding on phones */
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