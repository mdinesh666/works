---
layout: home
permalink: /
---

<style>
  /* --- 1. LAYOUT OVERRIDES --- */
  header.site-header { display: none !important; }
  footer.site-footer { display: none !important; }

  .wrapper {
    max-width: 1200px !important; 
    padding-left: 5% !important;
    padding-right: 5% !important;
  }

body {
  font-family: -apple-system, BlinkMacSystemFont, "Inter", "Segoe UI", Roboto, sans-serif;
  color: #111;
  background-color: #fff;
  /* Adds a subtle noise texture image */
  background-image: url("data:image/svg+xml,%3Csvg viewBox='0 0 200 200' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='noiseFilter'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.65' numOctaves='3' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23noiseFilter)' opacity='0.03'/%3E%3C/svg%3E");
  margin: 0;
}

  /* --- 2. CUSTOM NAVIGATION BAR --- */
  .custom-nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 30px 0;
    margin-bottom: 20px;
    position: relative;
  }

/* Wrapper to position the dot relative to the image */
.avatar-wrapper {
  position: relative;
  display: inline-block;
}

/* The Image */
.logo-img {
  border-radius: 14px; /* Smooth rounded square */
  width: 56px; /* Slightly smaller looks more premium */
  height: 56px;
  object-fit: cover;
  transition: transform 0.2s ease;
  border: 1px solid rgba(0,0,0,0.05); /* Subtle border definition */
}

/* Hover Effect: Slight zoom */
.nav-logo:hover .logo-img {
  transform: scale(1.05);
}

/* The Green Status Dot */
.status-badge {
  position: absolute;
  bottom: -2px;
  right: -2px;
  width: 14px;
  height: 14px;
  background-color: #10B981; /* Emerald Green */
  border: 2px solid #fff; /* White border separates it from avatar */
  border-radius: 50%;
  box-shadow: 0 0 0 0 rgba(16, 185, 129, 0.7);
  animation: pulse-green 2s infinite;
}

/* The Pulse Animation */
@keyframes pulse-green {
  0% {
    transform: scale(0.95);
    box-shadow: 0 0 0 0 rgba(16, 185, 129, 0.7);
  }
  70% {
    transform: scale(1);
    box-shadow: 0 0 0 6px rgba(16, 185, 129, 0);
  }
  100% {
    transform: scale(0.95);
    box-shadow: 0 0 0 0 rgba(16, 185, 129, 0);
  }
}

  .nav-links {
    display: flex;
    gap: 30px;
    align-items: center;
  }

  .nav-links a {
    color: #333;
    text-decoration: none;
    font-size: 0.95rem;
    font-weight: 500;
    transition: color 0.2s ease;
  }
  
  .nav-links a:hover { color: #000; }

  /* Hamburger Icon */
  .hamburger {
    display: none;
    cursor: pointer;
    flex-direction: column;
    gap: 6px;
    z-index: 101;
  }

  .hamburger span {
    width: 25px;
    height: 2px;
    background-color: #333;
    transition: all 0.3s ease;
  }

  /* --- 3. INTRO SECTION --- */
  .intro-section {
    padding: 80px 0;
    max-width: 700px;
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

  /* --- 4. WORK GRID --- */
  .work-section-title {
    font-weight: 500;
    font-size: 1.8rem;
    letter-spacing: -0.5px;
    margin-bottom: 25px;
    color: #111;
  }

  .project-grid {
    display: grid;
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
    height: 200px;
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

project-card h3 {
  margin: 0 0 10px 0;
  font-size: 1.25rem;
  font-weight: 500;
  color: #111;
  line-height: 1.3;
  display: flex;
  align-items: center;
  gap: 8px; /* Space for the arrow */
}

/* Create the arrow using CSS pseudo-element */
.project-card h3::after {
  content: "→";
  opacity: 0;
  transform: translateX(-10px);
  transition: all 0.3s ease;
  font-weight: 300;
}

/* On Card Hover, show and move the arrow */
.project-card:hover h3::after {
  opacity: 1;
  transform: translateX(0);
}

  .project-card p {
    font-size: 0.85rem;
    color: #666;
    margin: 0;
    line-height: 1.5;
  }

  /* --- 6. CUSTOM FOOTER (UPDATED) --- */
  .custom-footer {
    display: flex;
    justify-content: space-between; /* Pushes left and right content apart */
    align-items: center;
    padding: 60px 0 40px 0;
    margin-top: 40px;
    border-top: 1px solid #f0f0f0;
    font-size: 1rem;
    font-weight: 500;
  }

  .footer-left {
    display: flex;
    align-items: center;
  }

  .footer-right {
    font-size: 0.85rem;
    color: #888;
    font-weight: 400;
  }

  .custom-footer a {
    color: #111;
    text-decoration: none;
    transition: opacity 0.2s;
  }
  
  .custom-footer a:hover { opacity: 0.6; }

  /* The Circle Divider */
  .footer-divider {
    width: 4px;
    height: 4px;
    background-color: #111;
    border-radius: 50%;
    margin: 0 15px;
    display: inline-block;
  }

  /* --- RESPONSIVE CSS --- */
  @media (max-width: 900px) {
    .project-grid { grid-template-columns: repeat(2, 1fr); } 
    .wrapper { max-width: 100% !important; }
  }

  @media (max-width: 768px) {
    .hamburger { display: flex; }

    .nav-links {
      position: fixed;
      top: 0;
      right: 0;
      height: 100vh;
      width: 100%;
      background-color: rgba(255, 255, 255, 0.98);
      flex-direction: column;
      justify-content: center;
      gap: 40px;
      transform: translateY(-100%);
      transition: transform 0.4s cubic-bezier(0.4, 0, 0.2, 1);
      z-index: 100;
    }

    .nav-links.active { transform: translateY(0); }
    .nav-links a { font-size: 1.5rem; font-weight: 600; }
    
    .hamburger.open span:nth-child(1) { transform: rotate(45deg) translate(5px, 6px); }
    .hamburger.open span:nth-child(2) { opacity: 0; }
    .hamburger.open span:nth-child(3) { transform: rotate(-45deg) translate(5px, -6px); }
  }

  @media (max-width: 600px) {
    .project-grid { grid-template-columns: 1fr; } 
    .intro-section { padding: 50px 0; }
    .intro-title { font-size: 1.8rem; }
    
    /* Stack footer on mobile */
    .custom-footer {
      flex-direction: column;
      gap: 20px;
    }
  }

  /* Define the animation */
@keyframes fadeInUp {
  from { opacity: 0; transform: translateY(20px); }
  to { opacity: 1; transform: translateY(0); }
}

/* Apply to elements */
.intro-section, .work-section-title, .project-card, .custom-footer {
  animation: fadeInUp 0.8s ease-out forwards;
  opacity: 0; /* Start hidden */
}

/* Stagger the delays so they load one by one */
.custom-nav { animation-delay: 0s; }
.intro-section { animation-delay: 0.2s; }
.work-section-title { animation-delay: 0.4s; }
.project-card:nth-child(1) { animation-delay: 0.5s; }
.project-card:nth-child(2) { animation-delay: 0.6s; }
.project-card:nth-child(3) { animation-delay: 0.7s; }
.custom-footer { animation-delay: 0.9s; }
</style>

<nav class="custom-nav">
<a href="/" class="nav-logo">
  <div class="avatar-wrapper">
    <img src="./assets/avatar.png" alt="M Logo" class="logo-img">
    <div class="status-badge"></div>
  </div>
</a>

  <div class="hamburger" id="hamburger-btn">
    <span></span>
    <span></span>
    <span></span>
  </div>

  <div class="nav-links" id="nav-links">
    <a href="/illustrations">Illustrations</a>
    <a href="/about">About me</a>
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

<script>
  const hamburger = document.getElementById('hamburger-btn');
  const navLinks = document.getElementById('nav-links');

  hamburger.addEventListener('click', () => {
    navLinks.classList.toggle('active'); 
    hamburger.classList.toggle('open');
  });
</script>
