---
layout: home
permalink: /
---

<style>
  /* --- 1. LAYOUT OVERRIDES (Make it Wide) --- */
  
  /* Hides the default theme header to use our custom one */
  header.site-header { display: none !important; }

  /* Forces the main container to be wide enough for 3 cards */
  .wrapper {
    max-width: 1200px !important; 
    padding-left: 5% !important;
    padding-right: 5% !important;
  }

  body {
    font-family: -apple-system, BlinkMacSystemFont, "Inter", "Segoe UI", Roboto, sans-serif;
    color: #111;
    background: #fff;
  }

  /* --- 2. CUSTOM NAVIGATION BAR --- */
  .custom-nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 40px 0; /* Breathing room at the very top */
    margin-bottom: 20px;
  }

  .nav-logo {
    font-weight: 800;
    font-size: 1.5rem;
    color: #000;
    text-decoration: none;
    display: flex;
    align-items: center;
    gap: 10px;
  }

  /* Placeholder styles for your temp logo image */
  .logo-img {
    height: 40px; 
    width: auto;
  }

  .nav-links a {
    color: #333;
    text-decoration: none;
    margin-left: 30px;
    font-size: 0.95rem;
    font-weight: 500;
  }
  
  .nav-links a:hover { color: #000; }

  /* --- 3. INTRO SECTION --- */
  .intro-section {
    padding: 100px 0 80px 0; /* Large spacing top & bottom */
    max-width: 700px; /* Keeps text readable width */
  }

  .intro-title {
    font-size: 2.2rem;
    font-weight: 500;
    line-height: 1.2;
    margin-bottom: 1.5rem;
    letter-spacing: -0.5px;
    color: #000;
  }

  .intro-text {
    font-size: 1.15rem;
    line-height: 1.6;
    color: #555;
  }

  /* --- 4. WORK GRID (3 Columns) --- */
  
  .work-section-title {
    font-weight: 500;
    font-size: 1.8rem;
    letter-spacing: -0.5px;
    margin-bottom: 25px; /* Reduced space between title and cards */
    color: #111;
  }

  .project-grid {
    display: grid;
    /* Forces 3 columns. If screen is small, it auto-wraps */
    grid-template-columns: repeat(3, 1fr); 
    gap: 30px; 
    margin-bottom: 5rem;
  }

  /* --- 5. CARD DESIGN --- */
  .project-card {
    background: #ffffff;
    border: 1px solid rgba(0,0,0,0.08);
    border-radius: 12px;
    text-decoration: none !important;
    color: inherit;
    transition: transform 0.3s ease, box-shadow 0.3s ease;
    display: flex;
    flex-direction: column;
    overflow: hidden;
  }

  .project-card:hover {
    transform: translateY(-5px);
    box-shadow: 0 15px 30px rgba(0,0,0,0.1);
    border-color: rgba(0,0,0,0);
  }

  .card-img-container {
    height: 200px; /* Fixed height for consistency */
    background: #f4f4f4;
    overflow: hidden;
  }

  .card-img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    transition: transform 0.5s ease;
  }
  
  .project-card:hover .card-img { transform: scale(1.05); }

  .card-content {
    padding: 24px;
    display: flex;
    flex-direction: column;
    flex-grow: 1;
  }

  .project-date {
    font-size: 0.7rem;
    font-weight: 700;
    text-transform: uppercase;
    letter-spacing: 1.2px;
    color: #999;
    margin-bottom: 10px;
    display: block;
  }

  .project-card h3 {
    margin: 0 0 10px 0;
    font-size: 1.25rem;
    font-weight: 500;
    color: #111;
    line-height: 1.3;
  }

  .project-card p {
    font-size: 0.85rem;
    color: #666;
    margin: 0;
    line-height: 1.5;
  }

  /* --- RESPONSIVE MOBILE --- */
  @media (max-width: 900px) {
    .project-grid { grid-template-columns: repeat(2, 1fr); } /* 2 cols on tablet */
    .wrapper { max-width: 100% !important; }
  }

  @media (max-width: 600px) {
    .project-grid { grid-template-columns: 1fr; } /* 1 col on mobile */
    .intro-section { padding: 60px 0; }
    .intro-title { font-size: 1.8rem; }
  }
</style>

<nav class="custom-nav">
  <a href="/" class="nav-logo" width="100%">
    <img src="/assets/avatar.png" alt="M Logo" class="logo-img">
    </a>
  <div class="nav-links">
    <a href="/about">About</a>
    <a href="mailto:your@email.com">Contact</a>
  </div>
</nav>

<div class="intro-section">
  <h1 class="intro-title">Hi, I am Muthudinesh.</h1>
  <div class="intro-text">
   Product Designer at Congruent. By day, I build robust enterprise applications. By night, I tinker with electronics and AI. I bridge the gap between "it looks good" and "it actually works."
  </div>
</div>

<h2 class="work-section-title">Featured Works.</h2>

<div class="project-grid">

  <a href="https://medium.com/@muthudinesh666/from-pixels-to-perfect-code-the-architectural-blueprint-for-our-figma-to-code-agent-9004a6a4955e" class="project-card">
    <div class="card-img-container">
       <img src="https://miro.medium.com/v2/resize:fit:4800/format:webp/1*9K6lbAlqnOiszWskMRbLJA.png" alt="FigmaToCode Agent" class="card-img">
    </div>
    <div class="card-content">
      <span class="project-date">Oct 2025</span>
      <h3>FigmaToCode Agent</h3>
      <p>A minimalist pure navigation hardware device built for delivery partners using ESP32.</p>
    </div>
  </a> 

</div>
