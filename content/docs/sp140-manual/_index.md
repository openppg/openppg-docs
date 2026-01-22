---
title: "SP140 v2.5 User Manual"
description: "User Manual for the OpenPPG SP140 v2.5 Electric Paramotor"
weight: 1
---

<style>
.manual-hero {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 2rem;
  align-items: center;
  margin-bottom: 2rem;
  padding: 1.5rem 0;
}

.manual-hero-text {
  text-align: left;
}

.manual-hero-text h2 {
  font-size: 2rem;
  font-weight: 700;
  margin-bottom: 0.5rem;
  color: var(--body-color);
  line-height: 1.2;
}

.manual-hero-text .version {
  font-size: 0.9rem;
  color: var(--text-muted);
  margin-bottom: 1rem;
}

.manual-hero-text .description {
  font-size: 1rem;
  color: var(--text-muted);
  line-height: 1.6;
  margin-bottom: 1.5rem;
}

.manual-hero-image {
  text-align: center;
}

.manual-hero-image img {
  max-width: 280px;
  width: 100%;
  height: auto;
}

.section-header {
  text-align: center;
  margin-bottom: 1.5rem;
}

.section-header h2 {
  font-size: 1.5rem;
  font-weight: 600;
  margin-bottom: 0.5rem;
}

.section-header p {
  color: var(--text-muted);
  font-size: 0.95rem;
  max-width: 700px;
  margin: 0 auto;
}

.video-grid {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 1.5rem;
  margin: 1.5rem 0 2rem;
}

.video-card {
  background: var(--card-background, #f8f9fa);
  border: 1px solid var(--border-color, #e9ecef);
  border-radius: 12px;
  overflow: hidden;
  transition: all 0.3s ease;
  box-shadow: 0 2px 8px rgba(0,0,0,0.08);
}

.video-card:hover {
  transform: translateY(-4px);
  box-shadow: 0 12px 24px rgba(0,0,0,0.15);
  border-color: var(--link-color, #0969da);
}

.video-card h3 {
  font-size: 1rem;
  font-weight: 600;
  padding: 1rem 1.25rem 0.75rem;
  margin: 0;
  color: var(--body-color);
  text-align: center;
}

.video-card .video-wrapper {
  position: relative;
  padding-bottom: 56.25%; /* 16:9 aspect ratio */
  height: 0;
  overflow: hidden;
}

.video-card .video-wrapper iframe {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  border: 0;
}

.app-section {
  background: linear-gradient(135deg, var(--primary-color, #0969da) 0%, var(--primary-dark, #0550ae) 100%);
  border-radius: 12px;
  padding: 2rem;
  margin: 2rem 0;
  text-align: center;
  color: white;
  box-shadow: 0 8px 24px rgba(9, 105, 218, 0.2);
  position: relative;
}

.app-section .coming-soon-badge {
  display: inline-block;
  background: rgba(255, 255, 255, 0.2);
  color: white;
  font-size: 0.75rem;
  font-weight: 600;
  text-transform: uppercase;
  letter-spacing: 0.5px;
  padding: 0.35rem 0.75rem;
  border-radius: 20px;
  margin-bottom: 0.75rem;
  border: 1px solid rgba(255, 255, 255, 0.3);
}

.app-section h2 {
  color: white;
  font-size: 1.35rem;
  margin-bottom: 0.5rem;
}

.app-section p {
  color: rgba(255, 255, 255, 0.9);
  margin-bottom: 1.25rem;
  font-size: 0.9rem;
  max-width: 600px;
  margin-left: auto;
  margin-right: auto;
}

.app-section img {
  max-width: 160px;
  width: 100%;
  height: auto;
  margin: 0 auto;
  background: white;
  padding: 0.75rem;
  border-radius: 10px;
}

@media (max-width: 992px) {
  .manual-hero {
    grid-template-columns: 1fr;
    text-align: center;
  }

  .manual-hero-text {
    text-align: center;
  }

  .video-grid {
    grid-template-columns: 1fr;
  }
}

@media (max-width: 768px) {
  .manual-hero-text h2 {
    font-size: 1.75rem;
  }

  .manual-hero-image img {
    max-width: 220px;
  }

  .app-section {
    padding: 1.5rem;
  }
}
</style>

<div class="manual-hero">
  <div class="manual-hero-text">
    <p class="version">Version 1.01 • January 2026</p>
    <p class="description">Complete assembly and operation guide for your OpenPPG SP140 v2.5 electric paramotor. Watch the video tutorials below to get started safely.</p>
  </div>
  <div class="manual-hero-image">
    <img src="images/image28.png" alt="SP140 v2.5">
  </div>
</div>

---

<div class="section-header">
  <h2>Quick Start Video Tutorials</h2>
  <p>Watch these essential videos to learn how to safely assemble and operate your SP140 v2.5.</p>
</div>

<div class="video-grid">
  <div class="video-card">
    <h3>Frame Assembly</h3>
    <div class="video-wrapper">
      {{< youtube PScYGVZks_c >}}
    </div>
  </div>

  <div class="video-card">
    <h3>Power Pack Assembly</h3>
    <div class="video-wrapper">
      {{< youtube PScYGVZks_c >}}
    </div>
  </div>
</div>

---

<div class="app-section">
  <span class="coming-soon-badge">Coming Soon</span>
  <h2>OpenPPG Mobile App</h2>
  <p>The official OpenPPG app will provide real-time telemetry, flight logging, and system diagnostics for your SP140 v2.5. Stay tuned for the official release.</p>
</div>
