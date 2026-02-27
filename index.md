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
  --accent-dim: rgba(167, 139, 250, 0.12);
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
  max-width: 760px;
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

/* ─── Hero Section ─── */
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

.hero-intro {
  text-align: left;
}

.hero-content {
  max-width: 700px;
  text-align: center;
}

/* ─── Profile Photo + Music ─── */
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
  content: '↓';
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
  0%, 100% { box-shadow: 0 8px 32px rgba(0, 0, 0, 0.4), 0 0 0 0 rgba(167, 139, 250, 0.4); }
  50% { box-shadow: 0 8px 32px rgba(0, 0, 0, 0.4), 0 0 0 15px rgba(167, 139, 250, 0); }
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

/* ─── Ambient Effects ─── */
.ambient-container {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
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
  width: 400px;
  height: 400px;
  border-radius: 50%;
  filter: blur(120px);
  opacity: 0;
  pointer-events: none;
  z-index: -1;
  transition: opacity 1s ease;
}

.soft-glow.active { opacity: 0.15; }

.soft-glow:nth-child(1) {
  top: -200px;
  left: -200px;
  background: #a78bfa;
  animation: glowPulse 6s ease-in-out infinite;
}

.soft-glow:nth-child(2) {
  bottom: -200px;
  right: -200px;
  background: #8b5cf6;
  animation: glowPulse 6s ease-in-out infinite 3s;
}

@keyframes glowPulse {
  0%, 100% { opacity: 0.1; transform: scale(1); }
  50% { opacity: 0.2; transform: scale(1.1); }
}

/* ─── Hero Text ─── */
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

/* ─── CTA Buttons ─── */
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

/* ─── Timeline Section ─── */
.timeline-section {
  margin: 16px 0 80px;
}

.section-header {
  font-size: 0.85rem;
  font-weight: 600;
  color: var(--text-muted);
  text-transform: uppercase;
  letter-spacing: 0.14em;
  margin-bottom: 32px;
  padding-bottom: 12px;
  border-bottom: 1px solid var(--surface-border);
}

.timeline {
  position: relative;
  padding-left: 28px;
}

.timeline::before {
  content: '';
  position: absolute;
  left: 6px;
  top: 8px;
  bottom: 8px;
  width: 1.5px;
  background: var(--surface-border);
}

.timeline-item {
  position: relative;
  padding-bottom: 28px;
}

.timeline-item:last-child { padding-bottom: 0; }

.timeline-marker {
  position: absolute;
  left: -28px;
  top: 8px;
  width: 13px;
  height: 13px;
  background: var(--surface);
  border: 2.5px solid var(--surface-border-hover);
  border-radius: 50%;
  z-index: 1;
  transition: all 0.25s ease;
}

.timeline-item:hover .timeline-marker {
  border-color: var(--accent);
  background: var(--accent);
  box-shadow: 0 0 0 4px var(--accent-dim);
}

.timeline-content {
  background: var(--surface-elevated);
  border: 1px solid var(--surface-border);
  border-radius: 10px;
  padding: 18px 22px;
  transition: border-color 0.25s ease, transform 0.25s ease;
}

.timeline-content:hover {
  border-color: var(--surface-border-hover);
  transform: translateX(3px);
}

.timeline-date {
  font-family: 'JetBrains Mono', monospace;
  font-size: 0.72rem;
  font-weight: 500;
  color: var(--accent);
  letter-spacing: 0.03em;
}

.timeline-title {
  font-size: 1rem;
  font-weight: 600;
  color: #ffffff;
  margin: 5px 0 6px;
  line-height: 1.35;
}

.timeline-text {
  font-size: 0.88rem;
  color: var(--text-secondary);
  margin: 0;
  line-height: 1.6;
}

/* ─── Responsive ─── */
@media (max-width: 768px) {
  .home-container {
    padding: 0 20px;
  }

  .hero-section {
    padding: 36px 0 48px;
  }

  .hero-top {
    flex-direction: column;
    gap: 24px;
  }

  .hero-intro {
    text-align: center;
  }

  .hero-title {
    font-size: 2rem;
  }

  .hero-subtitle {
    font-size: 1.05rem;
  }

  .hero-image {
    width: 160px;
    height: 160px;
  }

  .music-caption {
    top: -38px;
    font-size: 0.72rem;
  }

  .timeline {
    padding-left: 24px;
  }

  .timeline-marker {
    left: -24px;
  }

  .timeline-content {
    padding: 16px 18px;
  }
}
</style>

<div class="home-container">

<!-- Ambient Elements -->
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

<!-- Hero -->
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

  <!-- Hidden YouTube Player -->
  <iframe
    id="bgMusic"
    width="0"
    height="0"
    src="https://www.youtube.com/embed/PL7AvEObPAM?enablejsapi=1&autoplay=0&loop=1&playlist=PL7AvEObPAM"
    frameborder="0"
    allow="autoplay; encrypted-media"
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
        events: { 'onReady': onPlayerReady }
      });
    }

    function onPlayerReady(event) {}

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

<!-- Journey Timeline -->
<section class="timeline-section">
  <h2 class="section-header">My Journey</h2>
  <div class="timeline">
    <div class="timeline-item">
      <div class="timeline-marker"></div>
      <div class="timeline-content">
        <span class="timeline-date">Aug 2022</span>
        <h3 class="timeline-title">Started at Norco College</h3>
        <p class="timeline-text">Associate of Science in Mathematics.</p>
      </div>
    </div>
    <div class="timeline-item">
      <div class="timeline-marker"></div>
      <div class="timeline-content">
        <span class="timeline-date">Feb 2023 – Jun 2025</span>
        <h3 class="timeline-title">Math & Computer Science Tutor</h3>
        <p class="timeline-text">Tutored students in Calculus, Statistics, and Computer Science at Norco College.</p>
      </div>
    </div>
    <div class="timeline-item">
      <div class="timeline-marker"></div>
      <div class="timeline-content">
        <span class="timeline-date">2023–2024</span>
        <h3 class="timeline-title">CCCAA Soccer</h3>
        <p class="timeline-text">Played soccer with Norco College.</p>
      </div>
    </div>
    <div class="timeline-item">
      <div class="timeline-marker"></div>
      <div class="timeline-content">
        <span class="timeline-date">May 2024 – Jul 2024</span>
        <h3 class="timeline-title">Data Science Research Intern</h3>
        <p class="timeline-text">California State University, Fullerton. Developed a UEFA Euro prediction model using Random Forests and ELO rating systems.</p>
      </div>
    </div>
    <div class="timeline-item">
      <div class="timeline-marker"></div>
      <div class="timeline-content">
        <span class="timeline-date">Summer 2025</span>
        <h3 class="timeline-title">Won Healthcare Hackathon</h3>
        <p class="timeline-text">ASA NYC x AI4Purpose.</p>
      </div>
    </div>
    <div class="timeline-item">
      <div class="timeline-marker"></div>
      <div class="timeline-content">
        <span class="timeline-date">Sep 2025</span>
        <h3 class="timeline-title">Transferred to UC San Diego</h3>
        <p class="timeline-text">Pursuing B.S. in Data Science with a minor in Mathematics.</p>
      </div>
    </div>
    <div class="timeline-item">
      <div class="timeline-marker"></div>
      <div class="timeline-content">
        <span class="timeline-date">Oct 2025 – Present</span>
        <h3 class="timeline-title">HDSI Lab 3.0 Fellow</h3>
        <p class="timeline-text">Developing interdisciplinary AI and robotics projects for K–12 education, including interactive hardware prototypes and sports-focused LLM applications.</p>
      </div>
    </div>
    <div class="timeline-item">
      <div class="timeline-marker"></div>
      <div class="timeline-content">
        <span class="timeline-date">Oct 2025 – Dec 2025</span>
        <h3 class="timeline-title">DS3 Project Member – EvoCharge</h3>
        <p class="timeline-text">Built a machine learning dashboard using Lasso Regression to predict EV charging costs and availability.</p>
      </div>
    </div>
    <div class="timeline-item">
      <div class="timeline-marker"></div>
      <div class="timeline-content">
        <span class="timeline-date">Fall 2025</span>
        <h3 class="timeline-title">Dino Cage Competition</h3>
        <p class="timeline-text">Shark Tank-style pitch competition.</p>
      </div>
    </div>
    <div class="timeline-item">
      <div class="timeline-marker"></div>
      <div class="timeline-content">
        <span class="timeline-date">Jan 2026 – Present</span>
        <h3 class="timeline-title">DS3 Consultant – CER Energy Dashboard</h3>
        <p class="timeline-text">Developing a real-time energy analytics dashboard for the UCSD Center for Energy Research.</p>
      </div>
    </div>
    <div class="timeline-item">
      <div class="timeline-marker"></div>
      <div class="timeline-content">
        <span class="timeline-date">Jan 2026 – Present</span>
        <h3 class="timeline-title">Data Science Intern – Southern California Edison</h3>
        <p class="timeline-text">SP&E team. Incoming Summer 2026 Intern.</p>
      </div>
    </div>
  </div>
</section>

</div>
