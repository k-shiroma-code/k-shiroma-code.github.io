---
title: Home
layout: default
permalink: /
---

<style>
@import url('https://fonts.googleapis.com/css2?family=DM+Sans:ital,opsz,wght@0,9..40,300;0,9..40,400;0,9..40,500;0,9..40,600;0,9..40,700&family=JetBrains+Mono:wght@400;500&display=swap');

.home-container {
  --accent: #a78bfa;
  --accent-soft: #c4b5fd;
  --accent-dim: rgba(167, 139, 250, 0.08);
  --surface: #0a0a0a;
  --surface-elevated: #111111;
  --surface-border: #1e1e1e;
  --surface-border-hover: #2a2a2a;
  --text-primary: #ececec;
  --text-secondary: #b0b0b0;
  --text-muted: #707070;
  font-family: 'DM Sans', -apple-system, BlinkMacSystemFont, sans-serif;
  color: var(--text-primary);
  line-height: 1.75;
  max-width: 720px;
  margin: 0 auto;
  padding: 0 24px;
}

.home-container h1,
.home-container h2,
.home-container h3 {
  font-family: 'DM Sans', -apple-system, BlinkMacSystemFont, sans-serif;
  font-weight: 600;
  letter-spacing: -0.025em;
  line-height: 1.3;
}

/* Hero Section */
.hero-section {
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 56px 0 72px;
}

.hero-top {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 44px;
  margin-bottom: 36px;
  width: 100%;
}

.hero-intro { text-align: left; }

.hero-content {
  max-width: 700px;
  text-align: center;
}

/* Profile Photo + Music */
.profile-container {
  position: relative;
  display: flex;
  flex-direction: column;
  align-items: center;
}

.music-caption {
  position: absolute;
  top: -42px;
  left: 50%;
  transform: translateX(-50%);
  white-space: nowrap;
  font-size: 0.78rem;
  color: var(--accent);
  font-weight: 500;
  letter-spacing: 0.02em;
  animation: bounce 2s ease-in-out infinite;
}

.music-caption::after {
  content: '\2193';
  display: block;
  text-align: center;
  font-size: 1.1rem;
  margin-top: 2px;
  animation: arrowBounce 1s ease-in-out infinite;
}

@keyframes bounce {
  0%, 100% { transform: translateX(-50%) translateY(0); }
  50% { transform: translateX(-50%) translateY(-5px); }
}

@keyframes arrowBounce {
  0%, 100% { transform: translateY(0); }
  50% { transform: translateY(4px); }
}

.hero-image {
  width: 200px;
  height: 200px;
  object-fit: cover;
  border-radius: 50%;
  border: 3px solid var(--surface-border);
  box-shadow: 0 8px 32px rgba(0, 0, 0, 0.5);
  flex-shrink: 0;
  transition: border-color 0.3s ease, transform 0.3s ease;
  cursor: pointer;
}

.hero-image:hover {
  border-color: var(--accent);
  transform: scale(1.03);
}

.hero-image.playing {
  border-color: var(--accent);
  animation: pulse 1.5s ease-in-out infinite;
}

@keyframes pulse {
  0%, 100% { box-shadow: 0 8px 32px rgba(0,0,0,0.4), 0 0 0 0 rgba(167,139,250,0.4); }
  50% { box-shadow: 0 8px 32px rgba(0,0,0,0.4), 0 0 0 15px rgba(167,139,250,0); }
}

.now-playing {
  margin-top: 12px;
  font-size: 0.78rem;
  color: var(--accent);
  opacity: 0;
  transition: opacity 0.3s ease;
  display: flex;
  align-items: center;
  gap: 6px;
  font-weight: 500;
}

.now-playing.visible { opacity: 1; }

.now-playing .bars {
  display: flex;
  gap: 2px;
  align-items: flex-end;
  height: 12px;
}

.now-playing .bar {
  width: 3px;
  background: var(--accent);
  animation: soundBar 0.5s ease-in-out infinite alternate;
}

.now-playing .bar:nth-child(1) { height: 4px; animation-delay: 0s; }
.now-playing .bar:nth-child(2) { height: 8px; animation-delay: 0.1s; }
.now-playing .bar:nth-child(3) { height: 6px; animation-delay: 0.2s; }
.now-playing .bar:nth-child(4) { height: 10px; animation-delay: 0.3s; }

@keyframes soundBar {
  0% { transform: scaleY(0.5); }
  100% { transform: scaleY(1); }
}

/* Ambient Effects */
.ambient-container {
  position: fixed;
  top: 0; left: 0;
  width: 100%; height: 100%;
  pointer-events: none;
  z-index: -1;
  overflow: hidden;
  opacity: 0;
  transition: opacity 1s ease;
}

.ambient-container.active { opacity: 1; }

.particle {
  position: absolute;
  background: var(--accent);
  border-radius: 50%;
  opacity: 0;
}

.particle:nth-child(odd) { width: 4px; height: 4px; }
.particle:nth-child(even) { width: 6px; height: 6px; }

.particle:nth-child(1) { left: 10%; animation: floatSlow 8s ease-in-out infinite; }
.particle:nth-child(2) { left: 25%; animation: floatSlow 10s ease-in-out infinite 1s; }
.particle:nth-child(3) { left: 40%; animation: floatSlow 9s ease-in-out infinite 2s; }
.particle:nth-child(4) { left: 55%; animation: floatSlow 11s ease-in-out infinite 0.5s; }
.particle:nth-child(5) { left: 70%; animation: floatSlow 8.5s ease-in-out infinite 1.5s; }
.particle:nth-child(6) { left: 85%; animation: floatSlow 10s ease-in-out infinite 2.5s; }

@keyframes floatSlow {
  0% { transform: translateY(100vh); opacity: 0; }
  10% { opacity: 0.5; }
  90% { opacity: 0.5; }
  100% { transform: translateY(-10vh); opacity: 0; }
}

.soft-glow {
  position: fixed;
  width: 400px; height: 400px;
  border-radius: 50%;
  filter: blur(120px);
  opacity: 0;
  pointer-events: none;
  z-index: -1;
  transition: opacity 1s ease;
}

.soft-glow.active { opacity: 0.15; }

.soft-glow:nth-child(1) {
  top: -200px; left: -200px;
  background: #a78bfa;
  animation: glowPulse 6s ease-in-out infinite;
}

.soft-glow:nth-child(2) {
  bottom: -200px; right: -200px;
  background: #8b5cf6;
  animation: glowPulse 6s ease-in-out infinite 3s;
}

@keyframes glowPulse {
  0%, 100% { opacity: 0.1; transform: scale(1); }
  50% { opacity: 0.2; transform: scale(1.1); }
}

/* Hero Text */
.hero-greeting {
  color: var(--accent);
  font-size: 0.85rem;
  font-weight: 600;
  text-transform: uppercase;
  letter-spacing: 0.12em;
  margin-bottom: 10px;
}

.hero-title {
  font-size: 2.6rem;
  font-weight: 700;
  color: #ffffff;
  margin: 0 0 6px 0;
  line-height: 1.15;
}

.hero-subtitle {
  font-size: 1.15rem;
  color: var(--text-secondary);
  margin-bottom: 0;
  font-weight: 400;
}

/* CTA Buttons */
.hero-buttons {
  display: flex;
  gap: 12px;
  flex-wrap: wrap;
  justify-content: center;
}

.btn {
  display: inline-flex;
  align-items: center;
  gap: 8px;
  font-weight: 500;
  font-size: 0.9rem;
  font-family: 'DM Sans', sans-serif;
  padding: 11px 22px;
  border-radius: 8px;
  text-decoration: none;
  transition: all 0.2s ease;
  letter-spacing: 0.01em;
}

.btn-primary {
  background: var(--accent);
  color: #0a0a0a;
  border: 1px solid var(--accent);
}

.btn-primary:hover {
  background: var(--accent-soft);
  border-color: var(--accent-soft);
  transform: translateY(-1px);
}

.btn-secondary {
  background: transparent;
  color: var(--text-primary);
  border: 1px solid var(--surface-border-hover);
}

.btn-secondary:hover {
  background: var(--accent);
  border-color: var(--accent);
  color: #0a0a0a;
}

/* ═══ ACCORDION ═══ */
.journey-section {
  margin: 16px 0 80px;
}

.section-header {
  font-size: 0.85rem;
  font-weight: 600;
  color: var(--text-muted);
  text-transform: uppercase;
  letter-spacing: 0.14em;
  margin-bottom: 20px;
}

.accordion {
  display: flex;
  flex-direction: column;
  gap: 6px;
}

.accordion-item {
  border: 1px solid var(--surface-border);
  border-radius: 10px;
  overflow: hidden;
  transition: border-color 0.3s ease;
}

.accordion-item:hover,
.accordion-item.open {
  border-color: var(--surface-border-hover);
}

.accordion-trigger {
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 18px 22px;
  background: var(--surface-elevated);
  border: none;
  cursor: pointer;
  text-align: left;
  font-family: 'DM Sans', sans-serif;
  transition: background 0.2s ease;
}

.accordion-trigger:hover {
  background: #151515;
}

.accordion-trigger-left {
  display: flex;
  align-items: center;
  gap: 14px;
}

.accordion-icon {
  width: 36px;
  height: 36px;
  border-radius: 8px;
  background: var(--accent-dim);
  display: flex;
  align-items: center;
  justify-content: center;
  flex-shrink: 0;
  transition: background 0.3s ease;
}

.accordion-item.open .accordion-icon {
  background: var(--accent);
}

.accordion-icon svg {
  width: 18px;
  height: 18px;
  stroke: var(--accent);
  stroke-width: 1.8;
  fill: none;
  transition: stroke 0.3s ease;
}

.accordion-item.open .accordion-icon svg {
  stroke: #0a0a0a;
}

.accordion-label {
  font-size: 1rem;
  font-weight: 600;
  color: #ffffff;
  line-height: 1.3;
}

.accordion-count {
  font-family: 'JetBrains Mono', monospace;
  font-size: 0.7rem;
  color: var(--text-muted);
  margin-left: 2px;
  font-weight: 400;
}

.accordion-chevron {
  width: 20px;
  height: 20px;
  stroke: var(--text-muted);
  stroke-width: 2;
  fill: none;
  flex-shrink: 0;
  transition: transform 0.3s ease, stroke 0.3s ease;
}

.accordion-item.open .accordion-chevron {
  transform: rotate(180deg);
  stroke: var(--accent);
}

.accordion-panel {
  max-height: 0;
  overflow: hidden;
  transition: max-height 0.35s ease;
}

.accordion-panel-inner {
  padding: 4px 22px 20px;
  background: var(--surface-elevated);
}

.journey-entry {
  padding: 14px 0;
  border-bottom: 1px solid var(--surface-border);
}

.journey-entry:last-child {
  border-bottom: none;
  padding-bottom: 0;
}

.journey-entry:first-child {
  padding-top: 8px;
}

.journey-date {
  font-family: 'JetBrains Mono', monospace;
  font-size: 0.7rem;
  font-weight: 500;
  color: var(--accent);
  letter-spacing: 0.03em;
  display: block;
  margin-bottom: 4px;
}

.journey-title {
  font-size: 0.92rem;
  font-weight: 600;
  color: var(--text-primary);
  margin: 0 0 3px 0;
  line-height: 1.35;
}

.journey-desc {
  font-size: 0.84rem;
  color: var(--text-secondary);
  margin: 0;
  line-height: 1.55;
}

/* Responsive */
@media (max-width: 768px) {
  .home-container { padding: 0 20px; }
  .hero-section { padding: 36px 0 48px; }
  .hero-top { flex-direction: column; gap: 24px; }
  .hero-intro { text-align: center; }
  .hero-title { font-size: 2rem; }
  .hero-subtitle { font-size: 1.05rem; }
  .hero-image { width: 160px; height: 160px; }
  .music-caption { top: -38px; font-size: 0.72rem; }
  .accordion-trigger { padding: 16px 18px; }
  .accordion-panel-inner { padding: 4px 18px 18px; }
}
</style>

<div class="home-container">

<div class="soft-glow" id="glow1"></div>
<div class="soft-glow" id="glow2"></div>

<div class="ambient-container" id="ambient">
  <div class="particle"></div>
  <div class="particle"></div>
  <div class="particle"></div>
  <div class="particle"></div>
  <div class="particle"></div>
  <div class="particle"></div>
</div>

<section class="hero-section">
  <div class="hero-top">
    <div class="profile-container">
      <span class="music-caption">Click for a surprise</span>
      <img
        src="{{ site.baseurl }}/assets/img/IMG_9510.jpg"
        alt="Kyle Shiroma"
        class="hero-image"
        id="profilePic"
        onclick="toggleMusic()"
      >
      <div class="now-playing" id="nowPlaying">
        <div class="bars">
          <div class="bar"></div>
          <div class="bar"></div>
          <div class="bar"></div>
          <div class="bar"></div>
        </div>
        <span>Now Playing</span>
      </div>
    </div>
    <div class="hero-intro">
      <p class="hero-greeting">Welcome</p>
      <h1 class="hero-title">Kyle Shiroma</h1>
      <p class="hero-subtitle">Data Science @ UC San Diego</p>
    </div>
  </div>

  <iframe
    id="bgMusic" width="0" height="0"
    src="https://www.youtube.com/embed/PL7AvEObPAM?enablejsapi=1&autoplay=0&loop=1&playlist=PL7AvEObPAM"
    frameborder="0" allow="autoplay; encrypted-media"
    style="position: absolute; visibility: hidden;"
  ></iframe>

  <script>
    let isPlaying = false;
    let player;
    const profilePic = document.getElementById('profilePic');
    const nowPlaying = document.getElementById('nowPlaying');
    const ambient = document.getElementById('ambient');
    const glow1 = document.getElementById('glow1');
    const glow2 = document.getElementById('glow2');

    var tag = document.createElement('script');
    tag.src = "https://www.youtube.com/iframe_api";
    var firstScriptTag = document.getElementsByTagName('script')[0];
    firstScriptTag.parentNode.insertBefore(tag, firstScriptTag);

    function onYouTubeIframeAPIReady() {
      player = new YT.Player('bgMusic', {
        events: { 'onReady': function() {} }
      });
    }

    function toggleMusic() {
      if (!player) return;
      if (isPlaying) {
        player.pauseVideo();
        profilePic.classList.remove('playing');
        nowPlaying.classList.remove('visible');
        ambient.classList.remove('active');
        glow1.classList.remove('active');
        glow2.classList.remove('active');
      } else {
        player.playVideo();
        profilePic.classList.add('playing');
        nowPlaying.classList.add('visible');
        ambient.classList.add('active');
        glow1.classList.add('active');
        glow2.classList.add('active');
      }
      isPlaying = !isPlaying;
    }
  </script>

  <div class="hero-content">
    <div class="hero-buttons">
      <a href="{{ '/projects/' | relative_url }}" class="btn btn-primary">
        <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><rect x="3" y="3" width="18" height="18" rx="2"/><path d="M3 9h18"/><path d="M9 21V9"/></svg>
        View Projects
      </a>
      <a href="{{ '/assets/pdf/Kyle_Shiroma_Resume_PW.pdf' | relative_url }}" target="_blank" rel="noopener" class="btn btn-secondary">
        <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"/><polyline points="14 2 14 8 20 8"/><line x1="16" y1="13" x2="8" y2="13"/><line x1="16" y1="17" x2="8" y2="17"/></svg>
        Resume
      </a>
    </div>
  </div>
</section>

<section class="journey-section">
  <h2 class="section-header">My Journey</h2>
  <div class="accordion">

    <div class="accordion-item">
      <button class="accordion-trigger" onclick="toggleAccordion(this)">
        <span class="accordion-trigger-left">
          <span class="accordion-icon">
            <svg viewBox="0 0 24 24"><path d="M22 10v6M2 10l10-5 10 5-10 5z"/><path d="M6 12v5c0 1.1 2.7 3 6 3s6-1.9 6-3v-5"/></svg>
          </span>
          <span class="accordion-label">Education <span class="accordion-count">&middot; 2</span></span>
        </span>
        <svg class="accordion-chevron" viewBox="0 0 24 24"><polyline points="6 9 12 15 18 9"/></svg>
      </button>
      <div class="accordion-panel">
        <div class="accordion-panel-inner">
          <div class="journey-entry">
            <span class="journey-date">Sep 2025 &ndash; Present</span>
            <h3 class="journey-title">UC San Diego</h3>
            <p class="journey-desc">B.S. in Data Science, Minor in Mathematics.</p>
          </div>
          <div class="journey-entry">
            <span class="journey-date">Aug 2022 &ndash; Jun 2025</span>
            <h3 class="journey-title">Norco College</h3>
            <p class="journey-desc">Associate of Science in Mathematics.</p>
          </div>
        </div>
      </div>
    </div>

    <div class="accordion-item">
      <button class="accordion-trigger" onclick="toggleAccordion(this)">
        <span class="accordion-trigger-left">
          <span class="accordion-icon">
            <svg viewBox="0 0 24 24"><rect x="2" y="7" width="20" height="14" rx="2"/><path d="M16 7V5a2 2 0 0 0-2-2h-4a2 2 0 0 0-2 2v2"/></svg>
          </span>
          <span class="accordion-label">Experience <span class="accordion-count">&middot; 3</span></span>
        </span>
        <svg class="accordion-chevron" viewBox="0 0 24 24"><polyline points="6 9 12 15 18 9"/></svg>
      </button>
      <div class="accordion-panel">
        <div class="accordion-panel-inner">
          <div class="journey-entry">
            <span class="journey-date">Jan 2026 &ndash; Present</span>
            <h3 class="journey-title">Data Analytics Intern &middot; Southern California Edison</h3>
            <p class="journey-desc">SP&amp;E team. Incoming Summer 2026 Intern.</p>
          </div>
          <div class="journey-entry">
            <span class="journey-date">Oct 2025 &ndash; Present</span>
            <h3 class="journey-title">HDSI Lab 3.0 Fellow &middot; UC San Diego</h3>
            <p class="journey-desc">Developing AI and robotics projects for K&ndash;12 education, including interactive hardware prototypes and sports-focused LLM applications.</p>
          </div>
          <div class="journey-entry">
            <span class="journey-date">May 2024 &ndash; Jul 2024</span>
            <h3 class="journey-title">Data Science Research Intern &middot; CSU Fullerton</h3>
            <p class="journey-desc">Built a UEFA Euro prediction model using Random Forests and ELO rating systems under Dr. Doina Bein.</p>
          </div>
        </div>
      </div>
    </div>

    <div class="accordion-item">
      <button class="accordion-trigger" onclick="toggleAccordion(this)">
        <span class="accordion-trigger-left">
          <span class="accordion-icon">
            <svg viewBox="0 0 24 24"><path d="M12 2L2 7l10 5 10-5-10-5z"/><path d="M2 17l10 5 10-5"/><path d="M2 12l10 5 10-5"/></svg>
          </span>
          <span class="accordion-label">Projects <span class="accordion-count">&middot; 2</span></span>
        </span>
        <svg class="accordion-chevron" viewBox="0 0 24 24"><polyline points="6 9 12 15 18 9"/></svg>
      </button>
      <div class="accordion-panel">
        <div class="accordion-panel-inner">
          <div class="journey-entry">
            <span class="journey-date">Jan 2026 &ndash; Present</span>
            <h3 class="journey-title">CER Energy Dashboard &middot; DS3 Consultant</h3>
            <p class="journey-desc">Building a real-time energy analytics dashboard for the UCSD Center for Energy Research to visualize international oil import dependencies.</p>
          </div>
          <div class="journey-entry">
            <span class="journey-date">Oct 2025 &ndash; Dec 2025</span>
            <h3 class="journey-title">EvoCharge &middot; DS3 Project Member</h3>
            <p class="journey-desc">Built a machine learning dashboard using Lasso Regression to predict EV charging costs and station availability.</p>
          </div>
        </div>
      </div>
    </div>

    <div class="accordion-item">
      <button class="accordion-trigger" onclick="toggleAccordion(this)">
        <span class="accordion-trigger-left">
          <span class="accordion-icon">
            <svg viewBox="0 0 24 24"><circle cx="12" cy="8" r="6"/><path d="M15.477 12.89L17 22l-5-3-5 3 1.523-9.11"/></svg>
          </span>
          <span class="accordion-label">Highlights <span class="accordion-count">&middot; 3</span></span>
        </span>
        <svg class="accordion-chevron" viewBox="0 0 24 24"><polyline points="6 9 12 15 18 9"/></svg>
      </button>
      <div class="accordion-panel">
        <div class="accordion-panel-inner">
          <div class="journey-entry">
            <span class="journey-date">Summer 2025</span>
            <h3 class="journey-title">Won Healthcare Hackathon</h3>
            <p class="journey-desc">ASA NYC x AI4Purpose.</p>
          </div>
          <div class="journey-entry">
            <span class="journey-date">Fall 2025</span>
            <h3 class="journey-title">Dino Cage Competition</h3>
            <p class="journey-desc">Shark Tank-style pitch competition.</p>
          </div>
          <div class="journey-entry">
            <span class="journey-date">2023&ndash;2024</span>
            <h3 class="journey-title">CCCAA Soccer &middot; Norco College</h3>
            <p class="journey-desc">Played competitive college soccer.</p>
          </div>
        </div>
      </div>
    </div>

  </div>
</section>

<script>
function toggleAccordion(trigger) {
  var item = trigger.parentElement;
  var panel = trigger.nextElementSibling;
  var isOpen = item.classList.contains('open');

  document.querySelectorAll('.accordion-item').forEach(function(el) {
    el.classList.remove('open');
    el.querySelector('.accordion-panel').style.maxHeight = null;
  });

  if (!isOpen) {
    item.classList.add('open');
    panel.style.maxHeight = panel.scrollHeight + 'px';
  }
}
</script>

</div>
