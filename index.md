---
layout: home 
permalink: /
---

<style>
  /* --- CSS STYLES --- */

  /* 1. The Grid Container (Keeps previous spacing fixes) */
  .about_sec{
    margin: 3rem 0;
  }
  .about_sec p{
    font-size: 1rem;
  }
  .project-grid {
    display: grid;
    grid-template-columns: 1fr 1fr; /* 2 equal columns */
    gap: 25px; /* Explicit gap between items */
    row-gap: 30px; /* Extra vertical breathing room */
    margin-top: 1rem;
    margin-bottom: 3rem;
  }

  /* 2. The Project Card Container */
  .project-card {
    background: #fff; /* White background looks cleaner with images */
    border: 1px solid #e5e5e5;
    border-radius: 12px; /* Slightly rounder corners */
    text-decoration: none !important;
    color: #333;
    transition: all 0.3s ease;
    height: 100%;
    display: flex;
    flex-direction: column;
    overflow: hidden; /* CRITICAL: Ensures image doesn't bleed out of rounded corners */
    box-shadow: 0 2px 5px rgba(0,0,0,0.05); /* Subtle base shadow */
  }

  /* Hover Effect */
  .project-card:hover {
    transform: translateY(-5px);
    box-shadow: 0 12px 20px rgba(0,0,0,0.1);
    border-color: #ddd;
  }

  /* 3. The New Cover Image Style */
  .card-img {
    width: 100%;
    height: 220px; /* FIXED HEIGHT ensures all cards align perfectly */
    object-fit: cover; /* "Cover" settings: crops image to fill inner box without stretching */
    display: block;
    border-bottom: 1px solid #f0f0f0;
  }

  /* 4. The New Content Container (holds the text) */
  .card-content {
    padding: 24px; /* Padding applied only to text area now */
    flex-grow: 1; /* Ensures cards are same height even with different text length */
    display: flex;
    flex-direction: column;
  }

  /* Typography updates */
  .project-card h3 {
    margin-top: 0;
    margin-bottom: 12px;
    font-size: 1.3rem;
    font-weight: 500;
    color: #111;
    line-height: 1.3;
  }

  .project-card p {
    font-size: 0.8rem;
    color: #555;
    margin-bottom: 0;
    line-height: 1.6;
  }

  .project-date {
    font-size: 0.8rem;
    text-transform: uppercase;
    letter-spacing: 1px;
    font-weight: 600;
    color: #888;
    margin-bottom: 12px;
    display: block;
  }

  /* Mobile Responsive */
  @media (max-width: 768px) {
    .project-grid {
      grid-template-columns: 1fr; /* 1 column on mobile */
      gap: 30px;
    }
    .card-img {
       height: 200px; /* Slightly shorter images on mobile */
    }
  }
</style>

<div class="about_sec">
  <p>Hi, I'm Muthudinesh. I'm a Product Designer at Congruent. By day, I build robust enterprise applications. By night, I tinker with electronics and AI. I bridge the gap between "it looks good" and "it actually works."</p>
</div>


<h2>My Works</h2>

<div class="project-grid">
    <a href="./figmacodegen-agent" class="project-card">
    <div class="card-content">
      <span class="project-date">Aug 2025</span>
      <h4>Figma to Code Agent</h4>
      <p>An AI experiment leveraging prompt engineering to automate design-to-dev handoffs.</p>
    </div>
    <img src="https://picsum.photos/id/3/600/400" alt="AI Code Interface" class="card-img">
  </a>
  
  <a href="./project-1" class="project-card">
    <div class="card-content">
      <span class="project-date">Oct 2025</span>
      <h4>Mapper</h4>
      <p>A minimalist pure navigation hardware device built for delivery partners using ESP32.</p>
    </div>
    <img src="https://picsum.photos/id/1/600/400" alt="GPS Device Prototype" class="card-img">
  </a>

  <a href="#" class="project-card">
    <div class="card-content">
      <span class="project-date">Sep 2025</span>
      <h4>Enterprise design system</h4>
      <p>Redesigning the HTML email template structure for better responsive behavior across clients.</p>
    </div>
    <img src="https://picsum.photos/id/2/600/400" alt="Responsive Email Designs" class="card-img">
  </a>


</div>
