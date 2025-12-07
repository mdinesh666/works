---
layout: home
title: About Me
permalink: /about/
---

<style>
  /* --- GLOBAL STYLES (Matches Home) --- */
  header.site-header, footer.site-footer { display: none !important; }

  .wrapper {
    max-width: 1200px !important; 
    padding-left: 5% !important;
    padding-right: 5% !important;
  }

  body {
    font-family: -apple-system, BlinkMacSystemFont, "Inter", "Segoe UI", Roboto, sans-serif;
    color: #111;
    background: #fff;
    margin: 0;
  }

  /* --- NAVIGATION (Exact Copy) --- */
  .custom-nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 30px 0;
    margin-bottom: 60px;
  }

  .nav-logo {
    display: flex;
    align-items: center;
    gap: 14px;
    text-decoration: none;
  }

  .logo-img {
    width: 52px; height: 52px;
    border-radius: 14px;
    object-fit: cover;
    border: 1px solid rgba(0,0,0,0.06);
    background: #f4f4f4;
  }

  .profile-info {
    display: flex;
    flex-direction: column;
    justify-content: center;
    gap: 4px;
  }

  .profile-name {
    font-size: 1.05rem;
    font-weight: 700;
    color: #222;
    line-height: 1.1;
    letter-spacing: -0.3px;
  }

  .status-chip {
    display: inline-flex; align-items: center; gap: 6px;
    background: rgba(0,0,0,0.03); padding: 3px 8px;
    border-radius: 12px; width: fit-content;
    font-size: 0.7rem; font-weight: 600;
  }
  
  .status-dot { width: 6px; height: 6px; border-radius: 50%; }
  
  /* Status: Open */
  .status-chip.open { color: #059669; background: rgba(16, 185, 129, 0.1); }
  .status-chip.open .status-dot { background-color: #10B981; }

  .nav-links { display: flex; gap: 30px; align-items: center; }
  .nav-links a { color: #333; text-decoration: none; font-size: 0.95rem; font-weight: 500; }
  .nav-links a:hover { color: #000; }

  /* Hamburger (Mobile) */
  .hamburger { display: none; cursor: pointer; flex-direction: column; gap: 6px; }
  .hamburger span { width: 25px; height: 2px; background-color: #333; transition: all 0.3s ease; }

  /* --- PAGE CONTENT STYLES --- */
  .page-container {
    max-width: 700px; /* Readable width for text */
    margin: 0 auto;   /* Center it */
  }

  /* Section Headers */
  .section-title {
    font-size: 2.2rem;
    font-weight: 700;
    letter-spacing: -0.5px;
    margin-bottom: 1.5rem;
    color: #111;
  }

  .section-subtitle {
    font-size: 1.5rem;
    font-weight: 600;
    margin-top: 4rem;
    margin-bottom: 2rem;
    color: #111;
    border-bottom: 1px solid #eee;
    padding-bottom: 10px;
  }

  /* Intro Text */
  .about-desc {
    font-size: 1.15rem;
    line-height: 1.7;
    color: #555;
    margin-bottom: 2rem;
  }

  /* --- TIMELINE COMPONENT --- */
  .timeline {
    position: relative;
    padding-left: 20px;
    border-left: 2px solid #f0f0f0; /* The vertical line */
  }

  .timeline-item {
    position: relative;
    margin-bottom: 45px;
  }

  /* The Dot on the line */
  .timeline-item::before {
    content: '';
    position: absolute;
    left: -27px; /* Adjust to sit on the line */
    top: 6px;
    width: 12px;
    height: 12px;
    background: #fff;
    border: 2px solid #333;
    border-radius: 50%;
  }

  .job-title {
    font-size: 1.2rem;
    font-weight: 700;
    color: #111;
    margin: 0 0 5px 0;
  }

  .job-meta {
    font-size: 0.85rem;
    font-weight: 600;
    color: #888;
    text-transform: uppercase;
    letter-spacing: 0.5px;
    margin-bottom: 10px;
    display: block;
  }

  .job-desc {
    font-size: 1rem;
    line-height: 1.6;
    color: #666;
    margin: 0;
  }

  /* --- FOOTER (Exact Copy) --- */
  .custom-footer {
    display: flex; justify-content: space-between; align-items: center;
    padding: 60px 0 40px 0; margin-top: 60px;
    border-top: 1px solid #f0f0f0; font-size: 1rem; font-weight: 500;
  }
  .footer-left { display: flex; align-items: center; }
  .footer-right { font-size: 0.85rem; color: #888; font-weight: 400; }
  .custom-footer a { color: #111; text-decoration: none; }
  .footer-divider { width: 4px; height: 4px; background-color: #111; border-radius: 50%; margin: 0 15px; }

  /* Mobile Responsive */
  @media (max-width: 768px) {
    .hamburger { display: flex; }
    .nav-links { display: none; } /* Add your mobile menu JS logic here if using same script */
    .section-title { font-size: 1.8rem; }
    .custom-footer { flex-direction: column; gap: 20px; }
  }
</style>

<nav class="custom-nav">
  <a href="/" class="nav-logo">
    <img src="/assets/avatar.png" alt="Muthudinesh" class="logo-img">
    <div class="profile-info">
      <span class="profile-name">Muthudinesh</span>
      <div class="status-chip open">
        <span class="status-dot"></span>
        <span class="status-text">Available</span>
      </div>
    </div>
  </a>

  <div class="hamburger">
    <span></span><span></span><span></span>
  </div>

  <div class="nav-links">
    <a href="/illustrations">Illustrations</a>
    <a href="/about" style="color: #000; font-weight: 700;">About me</a> <a href="mailto:your@email.com">Contact</a>
  </div>
</nav>

<div class="page-container">

  <h1 class="section-title">About me.</h1>
  <div class="about-desc">
    I design and deliver robust B2B enterprise applications by partnering closely with product management and software architects. From initial requirements to final release, I maintain rigorous accessibility standards while managing comprehensive design systems.
  </div>

  <h2 class="section-subtitle">Experience</h2>

  <div class="timeline">
    <div class="timeline-item">
      <h3 class="job-title">Product Designer</h3>
      <span class="job-meta">Mar 2023 - Present &nbsp;|&nbsp; Congruent Solutions • Chennai</span>
      <p class="job-desc">Leading design for 401(k) record-keeping products, implementing Web3 features, and maintaining the enterprise design system.</p>
    </div>
    <div class="timeline-item">
      <h3 class="job-title">Visual Designer</h3>
      <span class="job-meta">Jun 2022 - Jan 2023 &nbsp;|&nbsp; Accenture • Chennai</span>
      <p class="job-desc">Crafted high-fidelity UI assets and collaborated with global teams to ensure brand consistency across digital touchpoints.</p>
    </div>
    <div class="timeline-item">
      <h3 class="job-title">Visual Designer</h3>
      <span class="job-meta">Jun 2019 - Jun 2022 &nbsp;|&nbsp; Osiz Technologies • Madurai</span>
      <p class="job-desc">Designed user interfaces for crypto-exchange platforms and marketing collateral for blockchain-based products.</p>
    </div>
    <div class="timeline-item">
      <h3 class="job-title">Graphic Designer</h3>
      <span class="job-meta">Dec 2017 - Mar 2019 &nbsp;|&nbsp; Kevell Corp • Madurai</span>
      <p class="job-desc">Developed branding materials, social media graphics, and website layouts for early-stage startups.</p>
    </div>

  </div>

</div>

<footer class="custom-footer">
    <div class="footer-left">
        <a href="https://medium.com/@muthudinesh666" target="_blank">Medium</a>
        <span class="footer-divider"></span>
        <a href="https://linkedin.com/in/yourprofile" target="_blank">LinkedIn</a>
    </div>
    <div class="footer-right">
        Updated on {{ site.time | date: "%d %b" }}
    </div>
</footer>
