---
title: Home
layout: default
permalink: /
---

<style>
.home-container {
  --accent: #a78bfa;
  --accent-soft: #c4b5fd;
  --surface: #0a0a0a;
  --surface-elevated: #141414;
  --surface-border: #222;
  --text-primary: #f5f5f5;
  --text-secondary: #a0a0a0;
  --text-muted: #666;
  font-family: 'Manrope', -apple-system, BlinkMacSystemFont, sans-serif;
  color: var(--text-primary);
  line-height: 1.7;
}

.home-container h1,
.home-container h2,
.home-container h3 {
  font-family: 'Manrope', -apple-system, BlinkMacSystemFont, sans-serif;
  font-weight: 600;
  letter-spacing: -0.02em;
}

/* Hero Section */
.hero-section {
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 48px 0 64px;
}

.hero-top {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 48px;
  margin-bottom: 32px;
}

.hero-intro {
  text-align: left;
}

.hero-content {
  max-width: 700px;
  text-align: center;
}

/* Profile Photo with Music */
.profile-container {
  position: relative;
  display: flex;
  flex-direction: column;
  align-items: center;
}

.music-caption {
  position: absolute;
  top: -45px;
  left: 50%;
  transform: translateX(-50%);
  white-space: nowrap;
  font-size: 0.85rem;
  color: var(--accent);
  font-weight: 500;
  animation: bounce 2s ease-in-out infinite;
}

.music-caption::after {
  content: '↓';
  display: block;
  text-align: center;
  font-size: 1.2rem;
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
  width: 220px;
  height: 220px;
  object-fit: cover;
  border-radius: 50%;
  border: 4px solid var(--surface-border);
  box-shadow: 0 8px 32px rgba(0, 0, 0, 0.4);
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
  font-size: 0.8rem;
  color: var(--accent);
  opacity: 0;
  transition: opacity 0.3s ease;
  display: flex;
  align-items: center;
  gap: 6px;
}

.now-playing.visible {
  opacity: 1;
}

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

/* Lightshow Effects */
.lightshow-container {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  pointer-events: none;
  z-index: -1;
  overflow: hidden;
  opacity: 0;
  transition: opacity 0.5s ease;
}

.lightshow-container.active {
  opacity: 1;
}

.light-beam {
  position: absolute;
  width: 150px;
  height: 150%;
  top: -25%;
  background: linear-gradient(180deg, 
    transparent 0%, 
    var(--beam-color) 50%, 
    transparent 100%);
  opacity: 0.15;
  filter: blur(30px);
  transform-origin: top center;
}

.light-beam:nth-child(1) {
  --beam-color: #a78bfa;
  left: 10%;
  animation: beamSway1 3s ease-in-out infinite, beamPulse 1.5s ease-in-out infinite;
}

.light-beam:nth-child(2) {
  --beam-color: #c4b5fd;
  left: 30%;
  animation: beamSway2 4s ease-in-out infinite, beamPulse 2s ease-in-out infinite 0.3s;
}

.light-beam:nth-child(3) {
  --beam-color: #8b5cf6;
  left: 50%;
  animation: beamSway1 3.5s ease-in-out infinite reverse, beamPulse 1.8s ease-in-out infinite 0.6s;
}

.light-beam:nth-child(4) {
  --beam-color: #ddd6fe;
  left: 70%;
  animation: beamSway2 2.5s ease-in-out infinite, beamPulse 2.2s ease-in-out infinite 0.9s;
}

.light-beam:nth-child(5) {
  --beam-color: #a78bfa;
  left: 90%;
  animation: beamSway1 4s ease-in-out infinite, beamPulse 1.6s ease-in-out infinite 1.2s;
}

@keyframes beamSway1 {
  0%, 100% { transform: rotate(-15deg) translateX(0); }
  50% { transform: rotate(15deg) translateX(20px); }
}

@keyframes beamSway2 {
  0%, 100% { transform: rotate(10deg) translateX(0); }
  50% { transform: rotate(-20deg) translateX(-30px); }
}

@keyframes beamPulse {
  0%, 100% { opacity: 0.1; }
  50% { opacity: 0.25; }
}

/* Floating particles */
.particles-container {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  pointer-events: none;
  z-index: -1;
  overflow: hidden;
  opacity: 0;
  transition: opacity 0.5s ease;
}

.particles-container.active {
  opacity: 1;
}

.particle {
  position: absolute;
  width: 6px;
  height: 6px;
  background: var(--accent);
  border-radius: 50%;
  opacity: 0;
  animation: floatUp 4s ease-in-out infinite;
}

.particle:nth-child(1) { left: 5%; animation-delay: 0s; }
.particle:nth-child(2) { left: 15%; animation-delay: 0.5s; }
.particle:nth-child(3) { left: 25%; animation-delay: 1s; }
.particle:nth-child(4) { left: 35%; animation-delay: 1.5s; }
.particle:nth-child(5) { left: 45%; animation-delay: 2s; }
.particle:nth-child(6) { left: 55%; animation-delay: 0.3s; }
.particle:nth-child(7) { left: 65%; animation-delay: 0.8s; }
.particle:nth-child(8) { left: 75%; animation-delay: 1.3s; }
.particle:nth-child(9) { left: 85%; animation-delay: 1.8s; }
.particle:nth-child(10) { left: 95%; animation-delay: 2.3s; }

@keyframes floatUp {
  0% {
    transform: translateY(100vh) scale(0);
    opacity: 0;
  }
  10% {
    opacity: 0.8;
  }
  90% {
    opacity: 0.8;
  }
  100% {
    transform: translateY(-20vh) scale(1);
    opacity: 0;
  }
}

/* Radial pulse from center */
.pulse-ring {
  position: fixed;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  width: 100px;
  height: 100px;
  border: 2px solid var(--accent);
  border-radius: 50%;
  opacity: 0;
  pointer-events: none;
  z-index: -1;
}

.lightshow-active .pulse-ring {
  animation: expandPulse 2s ease-out infinite;
}

.pulse-ring:nth-child(2) { animation-delay: 0.5s; }
.pulse-ring:nth-child(3) { animation-delay: 1s; }

@keyframes expandPulse {
  0% {
    width: 100px;
    height: 100px;
    opacity: 0.6;
  }
  100% {
    width: 800px;
    height: 800px;
    opacity: 0;
  }
}

/* Background color shift */
body.lightshow-active {
  animation: bgColorShift 8s ease-in-out infinite;
}

@keyframes bgColorShift {
  0%, 100% { background-color: #0a0a0a; }
  25% { background-color: #0d0a12; }
  50% { background-color: #0a0a0f; }
  75% { background-color: #0f0a10; }
}

.hero-greeting {
  color: var(--accent);
  font-size: 1rem;
  font-weight: 600;
  text-transform: uppercase;
  letter-spacing: 0.1em;
  margin-bottom: 12px;
}

.hero-title {
  font-size: 2.75rem;
  font-weight: 700;
  color: var(--text-primary);
  margin: 0 0 8px 0;
  line-height: 1.2;
}

.hero-subtitle {
  font-size: 1.25rem;
  color: var(--text-secondary);
  margin-bottom: 24px;
}

.hero-description {
  color: var(--text-secondary);
  font-size: 1.05rem;
  margin-bottom: 32px;
  max-width: 540px;
}

.hero-description strong {
  color: var(--text-primary);
  font-weight: 600;
}

/* CTA Buttons */
.hero-buttons {
  display: flex;
  gap: 12px;
  flex-wrap: wrap;
}

.btn {
  display: inline-flex;
  align-items: center;
  gap: 8px;
  font-weight: 500;
  font-size: 0.95rem;
  padding: 12px 24px;
  border-radius: 8px;
  text-decoration: none;
  transition: all 0.2s ease;
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
  border: 1px solid var(--surface-border);
}

.btn-secondary:hover {
  background: var(--accent);
  border-color: var(--accent);
  color: #0a0a0a;
}

/* Info Cards */
.info-section {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 24px;
  margin: 48px 0;
}

.info-card {
  background: var(--surface-elevated);
  border: 1px solid var(--surface-border);
  border-radius: 16px;
  padding: 32px;
  transition: border-color 0.3s ease, transform 0.3s ease;
}

.info-card:hover {
  border-color: var(--accent);
  transform: translateY(-2px);
}

.info-card-icon {
  width: 48px;
  height: 48px;
  background: rgba(167, 139, 250, 0.1);
  border: 1px solid rgba(167, 139, 250, 0.3);
  border-radius: 12px;
  display: flex;
  align-items: center;
  justify-content: center;
  margin-bottom: 20px;
  color: var(--accent);
}

.info-card-title {
  font-size: 1.1rem;
  font-weight: 600;
  color: var(--text-primary);
  margin: 0 0 12px 0;
}

.info-card-text {
  color: var(--text-secondary);
  font-size: 0.95rem;
  margin: 0;
  line-height: 1.6;
}

/* Highlights */
.highlights-section {
  margin: 64px 0;
}

.section-header {
  font-size: 0.85rem;
  font-weight: 600;
  color: var(--text-muted);
  text-transform: uppercase;
  letter-spacing: 0.1em;
  margin-bottom: 24px;
}

.highlights-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  gap: 16px;
}

.highlight-item {
  background: rgba(255,255,255,0.03);
  border: 1px solid var(--surface-border);
  border-radius: 12px;
  padding: 24px;
  text-align: center;
  transition: border-color 0.3s ease;
}

.highlight-item:hover {
  border-color: var(--accent);
}

.highlight-value {
  font-size: 1.5rem;
  font-weight: 700;
  color: var(--accent);
  display: block;
}

.highlight-label {
  font-size: 0.8rem;
  color: var(--text-muted);
  text-transform: uppercase;
  letter-spacing: 0.05em;
  margin-top: 6px;
}

/* Responsive */
@media (max-width: 768px) {
  .hero-section {
    padding: 32px 0 48px;
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
    font-size: 1.1rem;
  }
  
  .hero-image {
    width: 180px;
    height: 180px;
  }
  
  .music-caption {
    top: -40px;
    font-size: 0.75rem;
  }
  
  .info-section {
    grid-template-columns: 1fr;
  }
}
</style>

<div class="home-container">

<!-- Lightshow Elements -->
<div class="lightshow-container" id="lightshow">
  <div class="light-beam"></div>
  <div class="light-beam"></div>
  <div class="light-beam"></div>
  <div class="light-beam"></div>
  <div class="light-beam"></div>
</div>

<div class="particles-container" id="particles">
  <div class="particle"></div>
  <div class="particle"></div>
  <div class="particle"></div>
  <div class="particle"></div>
  <div class="particle"></div>
  <div class="particle"></div>
  <div class="particle"></div>
  <div class="particle"></div>
  <div class="particle"></div>
  <div class="particle"></div>
</div>

<div class="pulse-ring"></div>
<div class="pulse-ring"></div>
<div class="pulse-ring"></div>

<!-- Hero Section -->
<section class="hero-section">
  <div class="hero-top">
    <div class="profile-container">
      <span class="music-caption">Click for epic music! 🎵</span>
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
    const lightshow = document.getElementById('lightshow');
    const particles = document.getElementById('particles');
    const body = document.body;
    
    // Load YouTube API
    var tag = document.createElement('script');
    tag.src = "https://www.youtube.com/iframe_api";
    var firstScriptTag = document.getElementsByTagName('script')[0];
    firstScriptTag.parentNode.insertBefore(tag, firstScriptTag);
    
    function onYouTubeIframeAPIReady() {
      player = new YT.Player('bgMusic', {
        events: {
          'onReady': onPlayerReady
        }
      });
    }
    
    function onPlayerReady(event) {
      // Player is ready
    }
    
    function toggleMusic() {
      if (!player) return;
      
      if (isPlaying) {
        player.pauseVideo();
        profilePic.classList.remove('playing');
        nowPlaying.classList.remove('visible');
        lightshow.classList.remove('active');
        particles.classList.remove('active');
        body.classList.remove('lightshow-active');
      } else {
        player.playVideo();
        profilePic.classList.add('playing');
        nowPlaying.classList.add('visible');
        lightshow.classList.add('active');
        particles.classList.add('active');
        body.classList.add('lightshow-active');
      }
      isPlaying = !isPlaying;
    }
  </script>
  
  <div class="hero-content">
    <p class="hero-description">
      Transfer student from <strong>Norco College</strong> pursuing a <strong>B.S. in Data Science</strong> with a planned <strong>minor in Mathematics</strong>. Currently a fellow with <strong>HDSI Lab 3.0</strong> and an active member of the <strong>Data Science Student Society (DS3)</strong>.
    </p>
    <div class="hero-buttons">
      <a href="{{ '/projects/' | relative_url }}" class="btn btn-primary">
        <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><rect x="3" y="3" width="18" height="18" rx="2"/><path d="M3 9h18"/><path d="M9 21V9"/></svg>
        View Projects
      </a>
      <a href="{{ '/assets/pdf/Kyle_Shiroma_Data_Science_Resume (1).pdf' | relative_url }}" target="_blank" rel="noopener" class="btn btn-secondary">
        <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"/><polyline points="14 2 14 8 20 8"/><line x1="16" y1="13" x2="8" y2="13"/><line x1="16" y1="17" x2="8" y2="17"/></svg>
        Resume
      </a>
    </div>
  </div>
</section>

<!-- Info Cards -->
<section class="info-section">
  <div class="info-card">
    <div class="info-card-icon">
      <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M22 10v6M2 10l10-5 10 5-10 5z"/><path d="M6 12v5c3 3 9 3 12 0v-5"/></svg>
    </div>
    <h3 class="info-card-title">Education</h3>
    <p class="info-card-text">B.S. Data Science at UC San Diego with a planned minor in Mathematics. Transferred from Norco College.</p>
  </div>
  
  <div class="info-card">
    <div class="info-card-icon">
      <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M12 20h9"/><path d="M16.5 3.5a2.121 2.121 0 0 1 3 3L7 19l-4 1 1-4L16.5 3.5z"/></svg>
    </div>
    <h3 class="info-card-title">Current Focus</h3>
    <p class="info-card-text">Machine learning, data analytics, and full-stack data applications with real-world impact.</p>
  </div>
  
  <div class="info-card">
    <div class="info-card-icon">
      <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M17 21v-2a4 4 0 0 0-4-4H5a4 4 0 0 0-4 4v2"/><circle cx="9" cy="7" r="4"/><path d="M23 21v-2a4 4 0 0 0-3-3.87"/><path d="M16 3.13a4 4 0 0 1 0 7.75"/></svg>
    </div>
    <h3 class="info-card-title">Involvement</h3>
    <p class="info-card-text">HDSI Lab 3.0 Fellow and DS3 member, contributing to the DataHacks event committee.</p>
  </div>
</section>

<!-- Highlights -->
<section class="highlights-section">
  <h2 class="section-header">Highlights</h2>
  <div class="highlights-grid">
    <div class="highlight-item">
      <span class="highlight-value">🏆</span>
      <span class="highlight-label">Hackathon Winner</span>
    </div>
    <div class="highlight-item">
      <span class="highlight-value">6+</span>
      <span class="highlight-label">Projects</span>
    </div>
    <div class="highlight-item">
      <span class="highlight-value">ML</span>
      <span class="highlight-label">Specialization</span>
    </div>
    <div class="highlight-item">
      <span class="highlight-value">UCSD</span>
      <span class="highlight-label">Data Science</span>
    </div>
  </div>
</section>

</div>
