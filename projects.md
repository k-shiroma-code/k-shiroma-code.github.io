---
title: Projects
layout: default
permalink: /projects/
---

<style>
.projects-container {
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

.projects-container h1,
.projects-container h2,
.projects-container h3 {
  font-family: 'Manrope', -apple-system, BlinkMacSystemFont, sans-serif;
  font-weight: 600;
  letter-spacing: -0.02em;
}

.project-card {
  background: var(--surface-elevated);
  border: 1px solid var(--surface-border);
  border-radius: 16px;
  padding: 40px;
  margin: 48px 0;
  transition: border-color 0.3s ease, transform 0.3s ease;
}

.project-card:hover {
  border-color: var(--accent);
  transform: translateY(-2px);
}

.project-header {
  display: flex;
  align-items: flex-start;
  justify-content: space-between;
  flex-wrap: wrap;
  gap: 16px;
  margin-bottom: 24px;
}

.project-title {
  font-size: 1.75rem;
  font-weight: 700;
  margin: 0;
  color: var(--text-primary);
}

.project-badge {
  display: inline-flex;
  align-items: center;
  gap: 6px;
  background: linear-gradient(135deg, var(--accent), var(--accent-soft));
  color: #0a0a0a;
  font-size: 0.75rem;
  font-weight: 600;
  text-transform: uppercase;
  letter-spacing: 0.05em;
  padding: 6px 14px;
  border-radius: 20px;
}

.project-description {
  color: var(--text-secondary);
  font-size: 1.05rem;
  margin-bottom: 28px;
  max-width: 720px;
}

.tech-stack {
  display: flex;
  flex-wrap: wrap;
  gap: 8px;
  margin-bottom: 24px;
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

.project-links {
  display: flex;
  flex-wrap: wrap;
  gap: 12px;
  margin-top: 24px;
}

.project-link {
  display: inline-flex;
  align-items: center;
  gap: 8px;
  color: var(--text-primary);
  text-decoration: none;
  font-weight: 500;
  font-size: 0.95rem;
  padding: 10px 20px;
  border: 1px solid var(--surface-border);
  border-radius: 8px;
  transition: all 0.2s ease;
}

.project-link:hover {
  background: var(--accent);
  border-color: var(--accent);
  color: #0a0a0a;
}

.project-link.primary {
  background: var(--accent);
  border-color: var(--accent);
  color: #0a0a0a;
}

.project-link.primary:hover {
  background: var(--accent-soft);
  border-color: var(--accent-soft);
}

/* Stats Grid */
.stats-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(140px, 1fr));
  gap: 16px;
  margin: 28px 0;
}

.stat-item {
  background: rgba(255,255,255,0.03);
  border: 1px solid var(--surface-border);
  border-radius: 12px;
  padding: 20px;
  text-align: center;
}

.stat-value {
  font-size: 1.6rem;
  font-weight: 700;
  color: var(--accent);
  display: block;
}

.stat-label {
  font-size: 0.75rem;
  color: var(--text-muted);
  text-transform: uppercase;
  letter-spacing: 0.08em;
  margin-top: 4px;
}

/* Model Table */
.model-table {
  width: 100%;
  border-collapse: collapse;
  margin: 20px 0;
  font-size: 0.9rem;
}

.model-table th {
  text-align: left;
  padding: 12px 16px;
  border-bottom: 2px solid var(--accent);
  color: var(--text-muted);
  font-weight: 600;
  text-transform: uppercase;
  font-size: 0.7rem;
  letter-spacing: 0.1em;
}

.model-table td {
  padding: 14px 16px;
  border-bottom: 1px solid var(--surface-border);
  color: var(--text-secondary);
}

.model-table tr:hover td {
  background: rgba(255,255,255,0.02);
}

.highlight-value {
  color: #22c55e;
  font-weight: 600;
}

/* Media Grid */
.media-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 20px;
  margin-top: 28px;
}

.media-item {
  border-radius: 12px;
  overflow: hidden;
  border: 1px solid var(--surface-border);
}

.media-item img {
  width: 100%;
  height: auto;
  display: block;
  transition: transform 0.4s ease;
}

.media-item:hover img {
  transform: scale(1.02);
}

/* Video Container */
.video-container {
  aspect-ratio: 16/9;
  border-radius: 12px;
  overflow: hidden;
  border: 1px solid var(--surface-border);
  background: #000;
}

.video-container video,
.video-container iframe {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

/* Layout Variants */
.project-layout-split {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 40px;
  align-items: start;
}

@media (max-width: 768px) {
  .project-layout-split {
    grid-template-columns: 1fr;
  }
  
  .project-card {
    padding: 24px;
    margin: 32px 0;
  }
  
  .project-title {
    font-size: 1.35rem;
  }
  
  .stats-grid {
    grid-template-columns: repeat(2, 1fr);
  }
  
  .media-grid {
    grid-template-columns: 1fr;
  }
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

/* Section Headers */
.section-header {
  font-size: 0.85rem;
  font-weight: 600;
  color: var(--text-muted);
  margin-bottom: 16px;
  text-transform: uppercase;
  letter-spacing: 0.1em;
}

/* Service Area List */
.service-list {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 8px;
  margin: 0;
  padding: 0;
  list-style: none;
}

.service-list li {
  color: var(--text-secondary);
  font-size: 0.9rem;
  padding: 8px 0;
  border-bottom: 1px solid var(--surface-border);
}

.service-list li strong {
  color: var(--accent-soft);
}

@media (max-width: 480px) {
  .service-list {
    grid-template-columns: 1fr;
  }
}

/* Tableau Embed */
.tableau-container {
  border-radius: 12px;
  overflow: hidden;
  border: 1px solid var(--surface-border);
  aspect-ratio: 16/9;
}

.tableau-container iframe {
  width: 100%;
  height: 100%;
  border: none;
}

/* Contribution Note */
.contribution-note {
  color: var(--text-muted);
  font-size: 0.9rem;
  margin-top: 20px;
  font-style: italic;
}
</style>

<div class="projects-container">

<div class="page-header">
  <h1>Projects</h1>
  <p>Machine learning, data analytics & full-stack development</p>
</div>

<!-- Weather & Energy Dashboard -->
<article class="project-card">
  <div class="project-header">
    <h2 class="project-title">Weather & Energy Dashboard</h2>
  </div>
  
  <p class="project-description">
    A full-stack web application featuring global weather data and California grid load forecasting using machine learning. The dashboard predicts 14-day electricity demand across 4 California service areas using ensemble models trained on 315,648 observations.
  </p>

  <div class="tech-stack">
    <span class="tech-tag">React</span>
    <span class="tech-tag">Astro</span>
    <span class="tech-tag">FastAPI</span>
    <span class="tech-tag">Python</span>
    <span class="tech-tag">scikit-learn</span>
    <span class="tech-tag">Recharts</span>
    <span class="tech-tag">OpenWeather API</span>
  </div>

  <div class="project-layout-split">
    <div>
      <h3 class="section-header">Model Performance</h3>
      <table class="model-table">
        <thead>
          <tr>
            <th>Model</th>
            <th>MAE</th>
            <th>MAPE</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>Gradient Boosting</td>
            <td class="highlight-value">573 MW</td>
            <td class="highlight-value">2.26%</td>
          </tr>
          <tr>
            <td>Random Forest</td>
            <td>577 MW</td>
            <td>2.29%</td>
          </tr>
          <tr>
            <td>Ridge + Weather</td>
            <td>840 MW</td>
            <td>3.41%</td>
          </tr>
        </tbody>
      </table>
    </div>
    <div>
      <h3 class="section-header">Service Areas</h3>
      <ul class="service-list">
        <li><strong>SCE</strong> — Southern California (15M people)</li>
        <li><strong>PG&E</strong> — Northern & Central CA (16M people)</li>
        <li><strong>SDG&E</strong> — San Diego Area (3.7M people)</li>
        <li><strong>VEA</strong> — Nevada/CA Border (45K people)</li>
      </ul>
    </div>
  </div>

  <div class="project-links">
    <a href="https://github.com/k-shiroma-code/Weather-API-Project" target="_blank" rel="noopener" class="project-link primary">
      <svg width="18" height="18" viewBox="0 0 24 24" fill="currentColor"><path d="M12 0c-6.626 0-12 5.373-12 12 0 5.302 3.438 9.8 8.207 11.387.599.111.793-.261.793-.577v-2.234c-3.338.726-4.033-1.416-4.033-1.416-.546-1.387-1.333-1.756-1.333-1.756-1.089-.745.083-.729.083-.729 1.205.084 1.839 1.237 1.839 1.237 1.07 1.834 2.807 1.304 3.492.997.107-.775.418-1.305.762-1.604-2.665-.305-5.467-1.334-5.467-5.931 0-1.311.469-2.381 1.236-3.221-.124-.303-.535-1.524.117-3.176 0 0 1.008-.322 3.301 1.23.957-.266 1.983-.399 3.003-.404 1.02.005 2.047.138 3.006.404 2.291-1.552 3.297-1.23 3.297-1.23.653 1.653.242 2.874.118 3.176.77.84 1.235 1.911 1.235 3.221 0 4.609-2.807 5.624-5.479 5.921.43.372.823 1.102.823 2.222v3.293c0 .319.192.694.801.576 4.765-1.589 8.199-6.086 8.199-11.386 0-6.627-5.373-12-12-12z"/></svg>
      View on GitHub
    </a>
  </div>
</article>

<!-- EvoCharge -->
<article class="project-card">
  <div class="project-header">
    <h2 class="project-title">EvoCharge</h2>
  </div>
  
  <p class="project-description">
    A machine-learning dashboard that predicts electric vehicle charging energy usage and cost across California. The system uses real-time Lasso regression powered by 3,500 charging sessions, 16,455 statewide stations, and county-level electricity rates.
  </p>

  <div class="tech-stack">
    <span class="tech-tag">Python</span>
    <span class="tech-tag">Streamlit</span>
    <span class="tech-tag">Lasso Regression</span>
    <span class="tech-tag">Figma</span>
    <span class="tech-tag">Data Visualization</span>
  </div>

  <div class="stats-grid">
    <div class="stat-item">
      <span class="stat-value">3,500</span>
      <span class="stat-label">Charging Sessions</span>
    </div>
    <div class="stat-item">
      <span class="stat-value">16,455</span>
      <span class="stat-label">CA Stations</span>
    </div>
    <div class="stat-item">
      <span class="stat-value">58</span>
      <span class="stat-label">County Rates</span>
    </div>
  </div>

  <div class="video-container">
    <video controls poster="{{ site.baseurl }}/assets/img/evocharge_screenshot.jpg">
      <source src="{{ site.baseurl }}/assets/img/EvoChargeDemo.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>

  <p class="contribution-note">
    My contributions: Website design in Figma, model testing and validation
  </p>

  <div class="project-links">
    <a href="https://evocharge.streamlit.app" target="_blank" rel="noopener" class="project-link primary">
      <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M18 13v6a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2V8a2 2 0 0 1 2-2h6"/><polyline points="15 3 21 3 21 9"/><line x1="10" y1="14" x2="21" y2="3"/></svg>
      Live App
    </a>
    <a href="https://github.com/anirudh9280/EvoCharge" target="_blank" rel="noopener" class="project-link">
      <svg width="18" height="18" viewBox="0 0 24 24" fill="currentColor"><path d="M12 0c-6.626 0-12 5.373-12 12 0 5.302 3.438 9.8 8.207 11.387.599.111.793-.261.793-.577v-2.234c-3.338.726-4.033-1.416-4.033-1.416-.546-1.387-1.333-1.756-1.333-1.756-1.089-.745.083-.729.083-.729 1.205.084 1.839 1.237 1.839 1.237 1.07 1.834 2.807 1.304 3.492.997.107-.775.418-1.305.762-1.604-2.665-.305-5.467-1.334-5.467-5.931 0-1.311.469-2.381 1.236-3.221-.124-.303-.535-1.524.117-3.176 0 0 1.008-.322 3.301 1.23.957-.266 1.983-.399 3.003-.404 1.02.005 2.047.138 3.006.404 2.291-1.552 3.297-1.23 3.297-1.23.653 1.653.242 2.874.118 3.176.77.84 1.235 1.911 1.235 3.221 0 4.609-2.807 5.624-5.479 5.921.43.372.823 1.102.823 2.222v3.293c0 .319.192.694.801.576 4.765-1.589 8.199-6.086 8.199-11.386 0-6.627-5.373-12-12-12z"/></svg>
      GitHub
    </a>
  </div>
</article>

<!-- Pulsepanion -->
<article class="project-card">
  <div class="project-header">
    <h2 class="project-title">Pulsepanion</h2>
    <span class="project-badge">🏆 1st Place — 2025 Ai4Purpose Hackathon</span>
  </div>
  
  <p class="project-description">
    An award-winning AI healthcare tool that analyzes eighteen months of patient data to generate actionable insights for caregivers. It applies natural language processing with large language models via the OpenAI API and presents results in an interactive R Shiny dashboard with PDF export functionality.
  </p>

  <div class="tech-stack">
    <span class="tech-tag">R Shiny</span>
    <span class="tech-tag">OpenAI API</span>
    <span class="tech-tag">NLP</span>
    <span class="tech-tag">Healthcare Analytics</span>
    <span class="tech-tag">PDF Export</span>
  </div>

  <div class="media-grid">
    <div class="media-item">
      <img src="{{ site.baseurl }}/assets/img/Pulsepantion.jpg" alt="Pulsepanion Dashboard">
    </div>
    <div class="video-container">
      <iframe 
        src="https://www.youtube.com/embed/tEJoXKLzVH4" 
        title="Pulsepanion Demo" 
        frameborder="0" 
        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" 
        allowfullscreen>
      </iframe>
    </div>
  </div>

  <div class="project-links">
    <a href="https://github.com/k-shiroma-code/NCHacks-Pulsepanion" target="_blank" rel="noopener" class="project-link primary">
      <svg width="18" height="18" viewBox="0 0 24 24" fill="currentColor"><path d="M12 0c-6.626 0-12 5.373-12 12 0 5.302 3.438 9.8 8.207 11.387.599.111.793-.261.793-.577v-2.234c-3.338.726-4.033-1.416-4.033-1.416-.546-1.387-1.333-1.756-1.333-1.756-1.089-.745.083-.729.083-.729 1.205.084 1.839 1.237 1.839 1.237 1.07 1.834 2.807 1.304 3.492.997.107-.775.418-1.305.762-1.604-2.665-.305-5.467-1.334-5.467-5.931 0-1.311.469-2.381 1.236-3.221-.124-.303-.535-1.524.117-3.176 0 0 1.008-.322 3.301 1.23.957-.266 1.983-.399 3.003-.404 1.02.005 2.047.138 3.006.404 2.291-1.552 3.297-1.23 3.297-1.23.653 1.653.242 2.874.118 3.176.77.84 1.235 1.911 1.235 3.221 0 4.609-2.807 5.624-5.479 5.921.43.372.823 1.102.823 2.222v3.293c0 .319.192.694.801.576 4.765-1.589 8.199-6.086 8.199-11.386 0-6.627-5.373-12-12-12z"/></svg>
      View on GitHub
    </a>
  </div>
</article>

<!-- Customer Segmentation -->
<article class="project-card">
  <div class="project-header">
    <h2 class="project-title">Customer Segmentation Analytics</h2>
  </div>
  
  <p class="project-description">
    A comprehensive analysis of over 500,000 retail transactions to uncover behavioral patterns in customer activity. Using RFM (Recency, Frequency, Monetary) analysis, the study identified five distinct customer segments, revealed seasonal purchasing trends, and optimized marketing spend allocation by 25%.
  </p>

  <div class="tech-stack">
    <span class="tech-tag">SQL</span>
    <span class="tech-tag">Tableau</span>
    <span class="tech-tag">Python</span>
    <span class="tech-tag">RFM Analysis</span>
    <span class="tech-tag">Data Visualization</span>
  </div>

  <div class="stats-grid">
    <div class="stat-item">
      <span class="stat-value">500K+</span>
      <span class="stat-label">Transactions</span>
    </div>
    <div class="stat-item">
      <span class="stat-value">5</span>
      <span class="stat-label">Segments</span>
    </div>
    <div class="stat-item">
      <span class="stat-value">25%</span>
      <span class="stat-label">Spend Optimization</span>
    </div>
  </div>

  <div class="tableau-container">
    <iframe 
      src="https://public.tableau.com/views/Customer_Segmentation_Overview_Github/Dashboard1?:showVizHome=no&:embed=true">
    </iframe>
  </div>

  <div class="project-links">
    <a href="https://github.com/k-shiroma-code/Customer-Segmentation-with-RFM-Analysis" target="_blank" rel="noopener" class="project-link primary">
      <svg width="18" height="18" viewBox="0 0 24 24" fill="currentColor"><path d="M12 0c-6.626 0-12 5.373-12 12 0 5.302 3.438 9.8 8.207 11.387.599.111.793-.261.793-.577v-2.234c-3.338.726-4.033-1.416-4.033-1.416-.546-1.387-1.333-1.756-1.333-1.756-1.089-.745.083-.729.083-.729 1.205.084 1.839 1.237 1.839 1.237 1.07 1.834 2.807 1.304 3.492.997.107-.775.418-1.305.762-1.604-2.665-.305-5.467-1.334-5.467-5.931 0-1.311.469-2.381 1.236-3.221-.124-.303-.535-1.524.117-3.176 0 0 1.008-.322 3.301 1.23.957-.266 1.983-.399 3.003-.404 1.02.005 2.047.138 3.006.404 2.291-1.552 3.297-1.23 3.297-1.23.653 1.653.242 2.874.118 3.176.77.84 1.235 1.911 1.235 3.221 0 4.609-2.807 5.624-5.479 5.921.43.372.823 1.102.823 2.222v3.293c0 .319.192.694.801.576 4.765-1.589 8.199-6.086 8.199-11.386 0-6.627-5.373-12-12-12z"/></svg>
      View on GitHub
    </a>
  </div>
</article>

<!-- Heart Disease Prediction -->
<article class="project-card">
  <div class="project-header">
    <h2 class="project-title">Heart Disease Prediction Pipeline</h2>
  </div>
  
  <p class="project-description">
    A machine learning pipeline that predicts cardiovascular risk using the UCI Heart Disease dataset. By addressing class imbalance with SMOTE and applying logistic regression, it achieved a 20% improvement in minority-class recall. The pipeline is designed for production deployment in healthcare analytics contexts.
  </p>

  <div class="tech-stack">
    <span class="tech-tag">Python</span>
    <span class="tech-tag">scikit-learn</span>
    <span class="tech-tag">SMOTE</span>
    <span class="tech-tag">Logistic Regression</span>
    <span class="tech-tag">Healthcare ML</span>
  </div>

  <div class="stats-grid">
    <div class="stat-item">
      <span class="stat-value">+20%</span>
      <span class="stat-label">Recall Improvement</span>
    </div>
    <div class="stat-item">
      <span class="stat-value">SMOTE</span>
      <span class="stat-label">Class Balancing</span>
    </div>
    <div class="stat-item">
      <span class="stat-value">UCI</span>
      <span class="stat-label">Dataset Source</span>
    </div>
  </div>

  <div class="media-grid">
    <div class="media-item">
      <img src="{{ site.baseurl }}/assets/img/IMG_1668.jpg" alt="Model Performance Metrics">
    </div>
    <div class="media-item">
      <img src="{{ site.baseurl }}/assets/img/Feature_Importance.jpg" alt="Feature Importance Analysis">
    </div>
  </div>

  <div class="project-links">
    <a href="https://github.com/k-shiroma-code/Heart-Disease-ML-Project" target="_blank" rel="noopener" class="project-link primary">
      <svg width="18" height="18" viewBox="0 0 24 24" fill="currentColor"><path d="M12 0c-6.626 0-12 5.373-12 12 0 5.302 3.438 9.8 8.207 11.387.599.111.793-.261.793-.577v-2.234c-3.338.726-4.033-1.416-4.033-1.416-.546-1.387-1.333-1.756-1.333-1.756-1.089-.745.083-.729.083-.729 1.205.084 1.839 1.237 1.839 1.237 1.07 1.834 2.807 1.304 3.492.997.107-.775.418-1.305.762-1.604-2.665-.305-5.467-1.334-5.467-5.931 0-1.311.469-2.381 1.236-3.221-.124-.303-.535-1.524.117-3.176 0 0 1.008-.322 3.301 1.23.957-.266 1.983-.399 3.003-.404 1.02.005 2.047.138 3.006.404 2.291-1.552 3.297-1.23 3.297-1.23.653 1.653.242 2.874.118 3.176.77.84 1.235 1.911 1.235 3.221 0 4.609-2.807 5.624-5.479 5.921.43.372.823 1.102.823 2.222v3.293c0 .319.192.694.801.576 4.765-1.589 8.199-6.086 8.199-11.386 0-6.627-5.373-12-12-12z"/></svg>
      View on GitHub
    </a>
  </div>
</article>

<!-- UEFA Euro 2024 -->
<article class="project-card">
  <div class="project-header">
    <h2 class="project-title">UEFA Euro 2024 Sports Analytics</h2>
  </div>
  
  <p class="project-description">
    A sports analytics project developing predictive models for UEFA Euro 2024 match outcomes by combining ELO-based ratings with traditional statistical features. Models such as Decision Trees, Random Forests, and XGBoost were trained and evaluated using precision, recall, and F1-score to identify the most effective approach.
  </p>

  <div class="tech-stack">
    <span class="tech-tag">Python</span>
    <span class="tech-tag">XGBoost</span>
    <span class="tech-tag">Random Forest</span>
    <span class="tech-tag">ELO Ratings</span>
    <span class="tech-tag">Sports Analytics</span>
  </div>

  <div class="media-grid">
    <div class="media-item">
      <img src="{{ site.baseurl }}/assets/img/IMG_1670.jpg" alt="UEFA Euro 2024 Prediction Visualization 1">
    </div>
    <div class="media-item">
      <img src="{{ site.baseurl }}/assets/img/IMG_1671.jpg" alt="UEFA Euro 2024 Prediction Visualization 2">
    </div>
  </div>

  <div class="project-links">
    <a href="https://github.com/k-shiroma-code/CSUF-REU-Football-Analytics" target="_blank" rel="noopener" class="project-link primary">
      <svg width="18" height="18" viewBox="0 0 24 24" fill="currentColor"><path d="M12 0c-6.626 0-12 5.373-12 12 0 5.302 3.438 9.8 8.207 11.387.599.111.793-.261.793-.577v-2.234c-3.338.726-4.033-1.416-4.033-1.416-.546-1.387-1.333-1.756-1.333-1.756-1.089-.745.083-.729.083-.729 1.205.084 1.839 1.237 1.839 1.237 1.07 1.834 2.807 1.304 3.492.997.107-.775.418-1.305.762-1.604-2.665-.305-5.467-1.334-5.467-5.931 0-1.311.469-2.381 1.236-3.221-.124-.303-.535-1.524.117-3.176 0 0 1.008-.322 3.301 1.23.957-.266 1.983-.399 3.003-.404 1.02.005 2.047.138 3.006.404 2.291-1.552 3.297-1.23 3.297-1.23.653 1.653.242 2.874.118 3.176.77.84 1.235 1.911 1.235 3.221 0 4.609-2.807 5.624-5.479 5.921.43.372.823 1.102.823 2.222v3.293c0 .319.192.694.801.576 4.765-1.589 8.199-6.086 8.199-11.386 0-6.627-5.373-12-12-12z"/></svg>
      View on GitHub
    </a>
  </div>
</article>

</div>
