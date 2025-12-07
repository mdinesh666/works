---
layout: home 
permalink: /illustrations/
---

<style>
  /* --- GLOBAL STYLES (Matches Home & About) --- */
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

  /* --- NAVIGATION --- */
  .custom-nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 30px 0;
    margin-bottom: 60px;
  }

  .nav-logo {
    display: flex; align-items: center; gap: 14px; text-decoration: none;
  }

  .logo-img {
    width: 52px; height: 52px; border-radius: 14px;
    object-fit: cover; border: 1px solid rgba(0,0,0,0.06); background: #f4f4f4;
  }

  .profile-info {
    display: flex; flex-direction: column; justify-content: center; gap: 4px;
  }

  .profile-name {
    font-size: 1.05rem; font-weight: 700; color: #222; line-height: 1.1; letter-spacing: -0.3px;
  }

  .status-chip {
    display: inline-flex; align-items: center; gap: 6px;
    background: rgba(0,0,0,0.03); padding: 3px 8px;
    border-radius: 12px; width: fit-content;
    font-size: 0.7rem; font-weight: 600;
  }
  
  .status-chip.open { color: #059669; background: rgba(16, 185, 129, 0.1); }
  .status-chip.open .status-dot { width: 6px; height: 6px; border-radius: 50%; background-color: #10B981; }

  .nav-links { display: flex; gap: 30px; align-items: center; }
  .nav-links a { color: #333; text-decoration: none; font-size: 0.95rem; font-weight: 500; }
  .nav-links a:hover { color: #000; }

  /* Hamburger */
  .hamburger { display: none; cursor: pointer; flex-direction: column; gap: 6px; }
  .hamburger span { width: 25px; height: 2px; background-color: #333; transition: all 0.3s ease; }

  /* --- MASONRY GRID STYLES --- */
  .page-header {
    margin-bottom: 40px;
    text-align: left;
  }

  .section-title {
    font-size: 2.2rem;
    font-weight: 500;
    letter-spacing: -0.5px;
    color: #111;
    margin-bottom: 10px;
  }

  .section-desc {
    font-size: 1.1rem;
    color: #666;
    max-width: 600px;
  }

  /* The Masonry Magic */
  .masonry-grid {
    column-count: 3; /* Creates 3 columns */
    column-gap: 20px; /* Space between columns */
  }

  .masonry-item {
    break-inside: avoid; /* Prevents image from being cut in half */
    margin-bottom: 20px; /* Space bottom */
    position: relative;
    border-radius: 8px;
    overflow: hidden;
    transition: transform 0.3s ease;
  }

  .masonry-item img {
    width: 100%;
    height: auto; /* Maintains aspect ratio */
    display: block;
    border-radius: 8px;
  }

  /* Hover Effect */
  .masonry-item:hover {
    transform: translateY(-5px);
    box-shadow: 0 10px 20px rgba(0,0,0,0.1);
    z-index: 2;
  }

  /* --- FOOTER --- */
  .custom-footer {
    display: flex; justify-content: space-between; align-items: center;
    padding: 60px 0 40px 0; margin-top: 60px;
    border-top: 1px solid #f0f0f0; font-size: 1rem; font-weight: 500;
  }
  .footer-left { display: flex; align-items: center; }
  .footer-right { font-size: 0.85rem; color: #888; font-weight: 400; }
  .custom-footer a { color: #111; text-decoration: none; }
  .footer-divider { width: 4px; height: 4px; background-color: #111; border-radius: 50%; margin: 0 15px; }

  /* Responsive Mobile */
  @media (max-width: 900px) {
    .masonry-grid { column-count: 2; } /* 2 columns on tablet */
  }
  @media (max-width: 600px) {
    .nav-links { display: none; }
    .hamburger { display: flex; }
    .masonry-grid { column-count: 1; } /* 1 column on mobile */
  }
</style>

<nav class="custom-nav">
  <a href="/works" class="nav-logo">
    <img src="{{ '/assets/avatar.png' | relative_url }}" alt="Muthudinesh" class="logo-img">
    <div class="profile-info">
      <span class="profile-name">Muthudinesh</span>
      <div class="status-chip open">
        <span class="status-dot"></span>
        <span class="status-text">OPEN TO WORK</span>
      </div>
    </div>
  </a>

  <div class="hamburger">
    <span></span><span></span><span></span>
  </div>

  <div class="nav-links">
    <a href="{{ '/illustrations/' | relative_url }}" style="color: #000; font-weight: 700;">Illustrations</a>
    <a href="{{ '/about/' | relative_url }}">About me</a>
    <a href="mailto:your@email.com">Contact</a>
  </div>
</nav>

<div class="page-header">
  <h1 class="section-title">Illustrations.</h1>
  <p class="section-desc">A collection of visual explorations, 3D renders, and vector art created during my free time.</p>
</div>

<div class="masonry-grid">

  <div class="masonry-item">
    <img src="{{ '/assets/1.jpg' | relative_url }}" alt="Illustration 1">
  </div>

  <div class="masonry-item">
    <img src="{{ '/assets/2.jpg' | relative_url }}" alt="Illustration 2">
  </div>

  <div class="masonry-item">
    <img src="{{ '/assets/3.jpg' | relative_url }}" alt="Illustration 3">
  </div>

  <div class="masonry-item">
    <img src="{{ '/assets/4.jpg' | relative_url }}" alt="Illustration 4">
  </div>

  <div class="masonry-item">
    <img src="{{ '/assets/5.jpg' | relative_url }}" alt="Illustration 5">
  </div>

  <div class="masonry-item">
    <img src="{{ '/assets/6.jpg' | relative_url }}" alt="Illustration 6">
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
