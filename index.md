---
title: Home
layout: default
permalink: /
---

<style>
.home-container {
  --accent: #e85d04;
  --accent-soft: #f48c06;
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

.hero-image {
  width: 220px;
  height: 220px;
  object-fit: cover;
  border-radius: 50%;
  border: 4px solid var(--surface-border);
  box-shadow: 0 8px 32px rgba(0, 0, 0, 0.4);
  flex-shrink: 0;
  transition: border-color 0.3s ease, transform 0.3s ease;
}

.hero-image:hover {
  border-color: var(--accent);
  transform: scale(1.03);
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
  color: #000;
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
  color: #000;
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
  background: rgba(232, 93, 4, 0.1);
  border: 1px solid rgba(232, 93, 4, 0.3);
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
  
  .info-section {
    grid-template-columns: 1fr;
  }
}
</style>

<div class="home-container">

<!-- Hero Section -->
<section class="hero-section">
  <div class="hero-top">
    <img 
      src="{{ site.baseurl }}/assets/img/IMG_9510.jpg" 
      alt="Kyle Shiroma"
      class="hero-image"
    >
    <div class="hero-intro">
      <p class="hero-greeting">Welcome</p>
      <h1 class="hero-title">Kyle Shiroma</h1>
      <p class="hero-subtitle">Data Science @ UC San Diego</p>
    </div>
  </div>
  
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
