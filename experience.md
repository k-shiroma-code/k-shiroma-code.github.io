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
}

.experience-container h1,
.experience-container h2,
.experience-container h3 {
  font-family: 'Manrope', -apple-system, BlinkMacSystemFont, sans-serif;
  font-weight: 600;
  letter-spacing: -0.02em;
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

<div class="experience-container">

<div class="page-header">
  <h1>Experience</h1>
  <p>Research, teaching & professional development</p>
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
        <p>
          Currently developing a full AI robotic flower using OpenCV for computer vision, which will serve as the foundation for a baseball card builder project. The system will capture photos of students and use LLMs to generate fun, personalized stats for their cards. Also helping build a curriculum to teach kids the basics of OpenAI and OpenCV through hands-on activities.
        </p>
        <p>
          Also contributing to a 3D fiber-optic installation with Arduino-controlled LEDs and 3D-printed linear actuators, presented through an interactive visual exhibit emphasizing hands-on learning. Supporting the development of a machine learning–assisted self-alignment system that automatically corrects fiber-optic misalignment—demonstrating hardware–software integration and applied ML in physical systems.
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
