---
title: Experience
layout: default
permalink: /experience/
---

<style>
.experience-container {
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
  position: relative;
  z-index: 1;
}

.experience-container h1,
.experience-container h2,
.experience-container h3 {
  font-family: 'Manrope', -apple-system, BlinkMacSystemFont, sans-serif;
  font-weight: 600;
  letter-spacing: -0.02em;
}

/* ═══ ELECTRICITY GRID BACKGROUND ═══ */
.grid-dots {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  pointer-events: none;
  z-index: 0;
  background-image: radial-gradient(circle, rgba(167, 139, 250, 0.15) 1px, transparent 1px);
  background-size: 48px 48px;
}

.grid-lines {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  pointer-events: none;
  z-index: 0;
  background-image:
    linear-gradient(rgba(167, 139, 250, 0.06) 1px, transparent 1px),
    linear-gradient(90deg, rgba(167, 139, 250, 0.06) 1px, transparent 1px);
  background-size: 48px 48px;
}

.grid-bg {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  pointer-events: none;
  z-index: 0;
  overflow: hidden;
}

.pulse-h, .pulse-v {
  position: fixed;
  pointer-events: none;
  z-index: 0;
  opacity: 0;
}

.pulse-h {
  height: 2px;
  left: 0;
  width: 100%;
  background: linear-gradient(90deg,
    transparent 0%,
    transparent 30%,
    rgba(167, 139, 250, 0.4) 45%,
    rgba(196, 181, 253, 0.7) 50%,
    rgba(167, 139, 250, 0.4) 55%,
    transparent 70%,
    transparent 100%
  );
  background-size: 200% 100%;
}

.pulse-v {
  width: 2px;
  top: 0;
  height: 100%;
  background: linear-gradient(180deg,
    transparent 0%,
    transparent 30%,
    rgba(167, 139, 250, 0.4) 45%,
    rgba(196, 181, 253, 0.7) 50%,
    rgba(167, 139, 250, 0.4) 55%,
    transparent 70%,
    transparent 100%
  );
  background-size: 100% 200%;
}

.pulse-h.fire {
  opacity: 1;
  animation: pulseSlideH 1.8s ease-out forwards;
}

.pulse-v.fire {
  opacity: 1;
  animation: pulseSlideV 1.8s ease-out forwards;
}

@keyframes pulseSlideH {
  0% { background-position: -100% 0; opacity: 1; }
  80% { opacity: 0.4; }
  100% { background-position: 200% 0; opacity: 0; }
}

@keyframes pulseSlideV {
  0% { background-position: 0 -100%; opacity: 1; }
  80% { opacity: 0.4; }
  100% { background-position: 0 200%; opacity: 0; }
}

.grid-node {
  position: fixed;
  width: 6px;
  height: 6px;
  border-radius: 50%;
  background: var(--accent);
  pointer-events: none;
  z-index: 0;
  opacity: 0;
}

.grid-node.flash {
  animation: nodeFlash 1.2s ease-out forwards;
}

@keyframes nodeFlash {
  0% { opacity: 0; transform: scale(0.5); box-shadow: 0 0 0 0 rgba(167, 139, 250, 0); }
  20% { opacity: 1; transform: scale(2); box-shadow: 0 0 16px 6px rgba(167, 139, 250, 0.4); }
  100% { opacity: 0; transform: scale(0.5); box-shadow: 0 0 0 0 rgba(167, 139, 250, 0); }
}

/* Page Header */
.page-header {
  text-align: center;
  padding: 48px 0 32px;
  margin-bottom: 20px;
}

.page-header h1 {
  font-size: 2.75rem;
  font-weight: 700;
  margin: 0;
  color: var(--text-primary);
}

.page-header p {
  color: var(--text-muted);
  font-size: 1.1rem;
  margin-top: 12px;
}

/* Experience Card */
.experience-card {
  background: var(--surface-elevated);
  border: 1px solid var(--surface-border);
  border-radius: 16px;
  padding: 40px;
  margin: 32px 0;
  transition: border-color 0.3s ease, transform 0.3s ease;
}

.experience-card:hover {
  border-color: var(--accent);
  transform: translateY(-2px);
}

.experience-layout {
  display: grid;
  grid-template-columns: 1fr;
  gap: 32px;
}

.experience-layout.with-image {
  grid-template-columns: 1fr 280px;
  align-items: center;
}

.experience-layout.image-left {
  grid-template-columns: 280px 1fr;
  align-items: center;
}

/* Header */
.experience-header {
  margin-bottom: 20px;
}

.experience-title {
  font-size: 1.5rem;
  font-weight: 700;
  color: var(--text-primary);
  margin: 0 0 8px 0;
}

.experience-meta {
  display: flex;
  align-items: center;
  gap: 16px;
  flex-wrap: wrap;
}

.experience-role {
  color: var(--accent);
  font-weight: 500;
  font-size: 0.95rem;
}

.experience-date {
  color: var(--text-muted);
  font-size: 0.9rem;
  display: flex;
  align-items: center;
  gap: 6px;
}

.experience-date svg {
  width: 14px;
  height: 14px;
}

/* Content */
.experience-content {
  color: var(--text-primary);
  font-size: 1rem;
}

.experience-content p {
  margin: 0 0 16px 0;
}

.experience-content p:last-child {
  margin-bottom: 0;
}

.experience-content strong {
  color: var(--text-primary);
  font-weight: 400;
}

/* Image */
.experience-image {
  border-radius: 12px;
  overflow: hidden;
  border: 1px solid var(--surface-border);
  width: 100%;
  height: fit-content;
}

.experience-image img {
  width: 100%;
  height: auto;
  display: block;
  transition: transform 0.4s ease;
}

.experience-image:hover img {
  transform: scale(1.02);
}

/* Tech Tags */
.tech-stack {
  display: flex;
  flex-wrap: wrap;
  gap: 8px;
  margin-top: 20px;
}

.tech-tag {
  background: rgba(167, 139, 250, 0.1);
  border: 1px solid rgba(167, 139, 250, 0.3);
  color: var(--accent-soft);
  font-size: 0.8rem;
  font-weight: 500;
  padding: 6px 12px;
  border-radius: 6px;
}

/* Stats */
.experience-stats {
  display: flex;
  gap: 24px;
  margin-top: 24px;
  padding-top: 24px;
  border-top: 1px solid var(--surface-border);
}

.stat {
  text-align: center;
}

.stat-value {
  font-size: 1.4rem;
  font-weight: 700;
  color: var(--accent);
  display: block;
}

.stat-label {
  font-size: 0.75rem;
  color: var(--text-muted);
  text-transform: uppercase;
  letter-spacing: 0.05em;
  margin-top: 4px;
}

/* Responsive */
@media (max-width: 768px) {
  .grid-dots, .grid-lines, .grid-bg { display: none; }

  .experience-layout.with-image,
  .experience-layout.image-left {
    grid-template-columns: 1fr;
  }
  
  .experience-layout.image-left .experience-image {
    order: -1;
  }
  
  .experience-card {
    padding: 24px;
    margin: 24px 0;
  }
  
  .experience-title {
    font-size: 1.25rem;
  }
  
  .experience-image {
    max-width: 280px;
  }
  
  .experience-stats {
    flex-wrap: wrap;
    gap: 16px;
  }
  
  .page-header h1 {
    font-size: 2rem;
  }
}
</style>

<div class="grid-dots"></div>
<div class="grid-lines"></div>
<div class="grid-bg" id="gridBg"></div>

<script>
(function() {
  var gridBg = document.getElementById('gridBg');
  var GRID = 48;

  function firePulse() {
    var isHorizontal = Math.random() > 0.5;
    var el = document.createElement('div');

    if (isHorizontal) {
      el.className = 'pulse-h';
      var row = Math.floor(Math.random() * (window.innerHeight / GRID)) * GRID;
      el.style.top = row + 'px';
    } else {
      el.className = 'pulse-v';
      var col = Math.floor(Math.random() * (window.innerWidth / GRID)) * GRID;
      el.style.left = col + 'px';
    }

    gridBg.appendChild(el);

    requestAnimationFrame(function() {
      el.classList.add('fire');
    });

    var nodeCount = Math.random() > 0.5 ? 2 : 1;
    for (var i = 0; i < nodeCount; i++) {
      (function(idx) {
        setTimeout(function() {
          var node = document.createElement('div');
          node.className = 'grid-node';
          if (isHorizontal) {
            node.style.top = (parseInt(el.style.top) - 3) + 'px';
            var randCol = Math.floor(Math.random() * (window.innerWidth / GRID)) * GRID;
            node.style.left = (randCol - 3) + 'px';
          } else {
            node.style.left = (parseInt(el.style.left) - 3) + 'px';
            var randRow = Math.floor(Math.random() * (window.innerHeight / GRID)) * GRID;
            node.style.top = (randRow - 3) + 'px';
          }
          gridBg.appendChild(node);
          requestAnimationFrame(function() { node.classList.add('flash'); });
          setTimeout(function() { node.remove(); }, 1400);
        }, 300 + idx * 400);
      })(i);
    }

    setTimeout(function() { el.remove(); }, 2000);
  }

  function scheduleNext() {
    var delay = 2000 + Math.random() * 4000;
    setTimeout(function() {
      firePulse();
      scheduleNext();
    }, delay);
  }

  setTimeout(function() {
    firePulse();
    scheduleNext();
  }, 800);
})();
</script>

<div class="experience-container">

<div class="page-header">
  <h1>Experience</h1>
  <p>Research, teaching & professional development</p>
</div>

<!-- Edison SCE Intern -->
<article class="experience-card">
  <div class="experience-layout">
    <div>
      <div class="experience-header">
        <h2 class="experience-title">Southern California Edison (SCE)</h2>
        <div class="experience-meta">
          <span class="experience-role">Incoming Intern – SP&E</span>
          <span class="experience-date">
            <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><rect x="3" y="4" width="18" height="18" rx="2"/><path d="M16 2v4M8 2v4M3 10h18"/></svg>
            Summer 2026
          </span>
        </div>
      </div>
      
      <div class="experience-content">
        <p>
          Incoming summer intern in the System Planning & Engineering (SP&E) division at Southern California Edison, one of the largest electric utilities in the United States serving approximately 15 million people across 50,000 square miles.
        </p>
        <p>
        </p>
      </div>
      
<!-- HDSI Research Fellow -->
<article class="experience-card">
  <div class="experience-layout">
    <div>
      <div class="experience-header">
        <h2 class="experience-title">UC San Diego HDSI 3.0 Lab</h2>
        <div class="experience-meta">
          <span class="experience-role">Undergraduate Research Fellow</span>
          <span class="experience-date">
            <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><rect x="3" y="4" width="18" height="18" rx="2"/><path d="M16 2v4M8 2v4M3 10h18"/></svg>
            2025 – Present
          </span>
        </div>
      </div>
      
      <div class="experience-content">
        <p>
          Working at the intersection of AI, engineering, and art to build K–12 educational engagement projects at the Halıcıoğlu Data Science Institute (HDSI) 3.0 Lab. The fellowship combines data science, robotics, and creative technologies with hands-on experience across multiple domains.
        </p>
      </div>
      
      <div class="tech-stack">
        <span class="tech-tag">Python</span>
        <span class="tech-tag">OpenCV</span>
        <span class="tech-tag">LLMs</span>
        <span class="tech-tag">Arduino</span>
        <span class="tech-tag">Raspberry Pi</span>
        <span class="tech-tag">3D Printing</span>
        <span class="tech-tag">React</span>
        <span class="tech-tag">Astro</span>
        <span class="tech-tag">Machine Learning</span>
      </div>
    </div>
  </div>
</article>

<!-- Norco College Tutoring -->
<article class="experience-card">
  <div class="experience-layout with-image">
    <div>
      <div class="experience-header">
        <h2 class="experience-title">Norco College Learning Resources Center</h2>
        <div class="experience-meta">
          <span class="experience-role">Peer Tutor</span>
          <span class="experience-date">
            <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><rect x="3" y="4" width="18" height="18" rx="2"/><path d="M16 2v4M8 2v4M3 10h18"/></svg>
            Jan 2023 – June 2025
          </span>
        </div>
      </div>
      
      <div class="experience-content">
        <p>
          Tutored over <strong>100 students</strong> in <strong>Calculus</strong>, <strong>Statistics</strong>, and <strong>C++</strong>, developing strong <strong>communication</strong> and <strong>mentoring skills</strong> while maintaining accurate documentation and timesheets.
        </p>
        <p>
          Guided students <strong>step-by-step through problem-solving</strong>, ensuring <strong>conceptual understanding</strong> and <strong>independent thinking</strong>. Helped students <strong>build confidence in STEM subjects</strong> and achieve their academic goals.
        </p>
      </div>
      
      <div class="tech-stack">
        <span class="tech-tag">Calculus</span>
        <span class="tech-tag">Statistics</span>
        <span class="tech-tag">C++</span>
        <span class="tech-tag">Mentoring</span>
        <span class="tech-tag">CRLA Certified</span>
      </div>
      
      <div class="experience-stats">
        <div class="stat">
          <span class="stat-value">100+</span>
          <span class="stat-label">Students Tutored</span>
        </div>
        <div class="stat">
          <span class="stat-value">2.5</span>
          <span class="stat-label">Years</span>
        </div>
        <div class="stat">
          <span class="stat-value">3</span>
          <span class="stat-label">Subjects</span>
        </div>
      </div>
    </div>
    
    <div class="experience-image">
      <img src="{{ site.baseurl }}/assets/img/IMG_1673.jpg" alt="CRLA Tutoring Certificate">
    </div>
  </div>
</article>

<!-- CSUF Data Science Intern -->
<article class="experience-card">
  <div class="experience-layout image-left">
    <div class="experience-image">
      <img src="{{ site.baseurl }}/assets/img/CSUF_DS.png" alt="CSUF Data Science Intern Project">
    </div>
    
    <div>
      <div class="experience-header">
        <h2 class="experience-title">CIC Summer Research Program</h2>
        <div class="experience-meta">
          <span class="experience-role">Data Science Intern</span>
          <span class="experience-date">
            <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><rect x="3" y="4" width="18" height="18" rx="2"/><path d="M16 2v4M8 2v4M3 10h18"/></svg>
            May – July 2024
          </span>
        </div>
      </div>
      
      <div class="experience-content">
        <p>
          Analyzed and structured <strong>European football match records</strong> through data cleaning, transformation, and Elo-based rating engineering. Built predictive models with <strong>Logistic Regression</strong> and <strong>XGBoost</strong>, achieving strong classification performance.
        </p>
        <p>
          Addressed class imbalance using <strong>SMOTE and undersampling</strong> techniques. Delivered insights through visual presentation to peers and program coordinators.
        </p>
      </div>
      
      <div class="tech-stack">
        <span class="tech-tag">Python</span>
        <span class="tech-tag">XGBoost</span>
        <span class="tech-tag">Logistic Regression</span>
        <span class="tech-tag">SMOTE</span>
        <span class="tech-tag">Data Visualization</span>
      </div>
      
      <div class="experience-stats">
        <div class="stat">
          <span class="stat-value">61%</span>
          <span class="stat-label">Accuracy</span>
        </div>
        <div class="stat">
          <span class="stat-value">+20%</span>
          <span class="stat-label">Recall Improvement</span>
        </div>
      </div>
    </div>
  </div>
</article>

</div>
