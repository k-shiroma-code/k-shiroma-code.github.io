---
title: Ongoing Projects
layout: default
permalink: /ongoing-projects/
description: A showcase of active development projects!
---

<style>
.ongoing-container {
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

.ongoing-container h1,
.ongoing-container h2,
.ongoing-container h3 {
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

/* Project Card */
.project-card {
  background: var(--surface-elevated);
  border: 1px solid var(--surface-border);
  border-radius: 16px;
  padding: 40px;
  margin: 32px 0;
  transition: border-color 0.3s ease, transform 0.3s ease;
  position: relative;
  overflow: hidden;
}

.project-card:hover {
  border-color: var(--accent);
  transform: translateY(-2px);
}

/* Status Badge */
.status-badge {
  display: inline-flex;
  align-items: center;
  gap: 6px;
  font-size: 0.75rem;
  font-weight: 600;
  text-transform: uppercase;
  letter-spacing: 0.05em;
  padding: 6px 14px;
  border-radius: 20px;
  margin-bottom: 16px;
}

.status-badge.upcoming {
  background: rgba(59, 130, 246, 0.15);
  border: 1px solid rgba(59, 130, 246, 0.4);
  color: #60a5fa;
}

.status-badge.in-progress {
  background: rgba(34, 197, 94, 0.15);
  border: 1px solid rgba(34, 197, 94, 0.4);
  color: #4ade80;
}

.status-badge svg {
  width: 14px;
  height: 14px;
}

/* Project Header */
.project-header {
  margin-bottom: 20px;
}

.project-title {
  font-size: 1.5rem;
  font-weight: 700;
  color: var(--text-primary);
  margin: 0;
}

/* Project Content */
.project-description {
  color: var(--text-secondary);
  font-size: 1.05rem;
  margin-bottom: 24px;
  max-width: 720px;
}

.project-description strong {
  color: var(--text-primary);
  font-weight: 600;
}

/* Features List */
.features-section {
  margin: 24px 0;
}

.features-label {
  font-size: 0.85rem;
  font-weight: 600;
  color: var(--text-muted);
  text-transform: uppercase;
  letter-spacing: 0.1em;
  margin-bottom: 16px;
}

.features-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 12px;
}

.feature-item {
  display: flex;
  align-items: flex-start;
  gap: 12px;
  padding: 16px;
  background: rgba(255, 255, 255, 0.02);
  border: 1px solid var(--surface-border);
  border-radius: 10px;
  transition: border-color 0.2s ease;
}

.feature-item:hover {
  border-color: rgba(232, 93, 4, 0.4);
}

.feature-icon {
  width: 32px;
  height: 32px;
  background: rgba(232, 93, 4, 0.1);
  border: 1px solid rgba(232, 93, 4, 0.3);
  border-radius: 8px;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-shrink: 0;
  color: var(--accent);
}

.feature-icon svg {
  width: 16px;
  height: 16px;
}

.feature-text {
  color: var(--text-secondary);
  font-size: 0.95rem;
  line-height: 1.5;
}

.feature-text strong {
  color: var(--text-primary);
  font-weight: 600;
}

/* Tech Stack */
.tech-stack {
  display: flex;
  flex-wrap: wrap;
  gap: 8px;
  margin-top: 24px;
}

.tech-tag {
  background: rgba(232, 93, 4, 0.1);
  border: 1px solid rgba(232, 93, 4, 0.3);
  color: var(--accent-soft);
  font-size: 0.8rem;
  font-weight: 500;
  padding: 6px 12px;
  border-radius: 6px;
}

/* Timeline Indicator */
.timeline-indicator {
  display: flex;
  align-items: center;
  gap: 8px;
  margin-top: 24px;
  padding-top: 24px;
  border-top: 1px solid var(--surface-border);
  color: var(--text-muted);
  font-size: 0.9rem;
}

.timeline-indicator svg {
  width: 16px;
  height: 16px;
  color: var(--accent);
}

/* Responsive */
@media (max-width: 768px) {
  .project-card {
    padding: 24px;
    margin: 24px 0;
  }
  
  .project-title {
    font-size: 1.25rem;
  }
  
  .features-grid {
    grid-template-columns: 1fr;
  }
  
  .page-header h1 {
    font-size: 2rem;
  }
}
</style>

<div class="ongoing-container">

<div class="page-header">
  <h1>Ongoing & Upcoming</h1>
  <p>Active development and future projects</p>
</div>

<!-- Image Classification -->
<article class="project-card">
  <span class="status-badge upcoming">
    <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><circle cx="12" cy="12" r="10"/><polyline points="12 6 12 12 16 14"/></svg>
    Upcoming
  </span>
  
  <div class="project-header">
    <h2 class="project-title">Image Classification with PyTorch</h2>
  </div>
  
  <p class="project-description">
    Building a <strong>deep learning image classification system</strong> using <strong>PyTorch</strong> and <strong>convolutional neural networks (CNNs)</strong>. The project will explore <strong>transfer learning techniques</strong>, <strong>model optimization</strong>, and <strong>deployment strategies</strong> for real-world computer vision applications.
  </p>
  
  <div class="features-section">
    <p class="features-label">Planned Features</p>
    <div class="features-grid">
      <div class="feature-item">
        <div class="feature-icon">
          <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M12 2L2 7l10 5 10-5-10-5z"/><path d="M2 17l10 5 10-5"/><path d="M2 12l10 5 10-5"/></svg>
        </div>
        <span class="feature-text"><strong>Custom CNN architecture</strong> with transfer learning from pre-trained models</span>
      </div>
      <div class="feature-item">
        <div class="feature-icon">
          <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><rect x="3" y="3" width="18" height="18" rx="2"/><circle cx="8.5" cy="8.5" r="1.5"/><path d="M21 15l-5-5L5 21"/></svg>
        </div>
        <span class="feature-text"><strong>Data augmentation pipeline</strong> for robust training</span>
      </div>
      <div class="feature-item">
        <div class="feature-icon">
          <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M22 12h-4l-3 9L9 3l-3 9H2"/></svg>
        </div>
        <span class="feature-text"><strong>Model evaluation</strong> and performance metrics</span>
      </div>
      <div class="feature-item">
        <div class="feature-icon">
          <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><circle cx="12" cy="12" r="10"/><line x1="2" y1="12" x2="22" y2="12"/><path d="M12 2a15.3 15.3 0 0 1 4 10 15.3 15.3 0 0 1-4 10 15.3 15.3 0 0 1-4-10 15.3 15.3 0 0 1 4-10z"/></svg>
        </div>
        <span class="feature-text"><strong>Web-based inference interface</strong> for real-time predictions</span>
      </div>
    </div>
  </div>
  
  <div class="tech-stack">
    <span class="tech-tag">Python</span>
    <span class="tech-tag">PyTorch</span>
    <span class="tech-tag">TorchVision</span>
    <span class="tech-tag">OpenCV</span>
    <span class="tech-tag">FastAPI</span>
  </div>
  
  <div class="timeline-indicator">
    <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><rect x="3" y="4" width="18" height="18" rx="2"/><path d="M16 2v4M8 2v4M3 10h18"/></svg>
    Starting Soon
  </div>
</article>

<!-- AI Agents -->
<article class="project-card">
  <span class="status-badge upcoming">
    <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><circle cx="12" cy="12" r="10"/><polyline points="12 6 12 12 16 14"/></svg>
    Upcoming
  </span>
  
  <div class="project-header">
    <h2 class="project-title">AI Agents with Natural Language Processing</h2>
  </div>
  
  <p class="project-description">
    Developing <strong>intelligent conversational agents</strong> powered by <strong>natural language processing (NLP)</strong> and <strong>large language models</strong>. The project will focus on building <strong>context-aware dialogue systems</strong> that can understand user intent, maintain conversation history, and perform task-oriented actions.
  </p>
  
  <div class="features-section">
    <p class="features-label">Planned Features</p>
    <div class="features-grid">
      <div class="feature-item">
        <div class="feature-icon">
          <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M21 15a2 2 0 0 1-2 2H7l-4 4V5a2 2 0 0 1 2-2h14a2 2 0 0 1 2 2z"/></svg>
        </div>
        <span class="feature-text"><strong>Multi-turn conversation management</strong> with context retention</span>
      </div>
      <div class="feature-item">
        <div class="feature-icon">
          <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><circle cx="11" cy="11" r="8"/><path d="M21 21l-4.35-4.35"/></svg>
        </div>
        <span class="feature-text"><strong>Intent recognition</strong> and entity extraction</span>
      </div>
      <div class="feature-item">
        <div class="feature-icon">
          <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"/><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"/></svg>
        </div>
        <span class="feature-text"><strong>Integration with external APIs</strong> and tools</span>
      </div>
      <div class="feature-item">
        <div class="feature-icon">
          <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M21 16V8a2 2 0 0 0-1-1.73l-7-4a2 2 0 0 0-2 0l-7 4A2 2 0 0 0 3 8v8a2 2 0 0 0 1 1.73l7 4a2 2 0 0 0 2 0l7-4A2 2 0 0 0 21 16z"/></svg>
        </div>
        <span class="feature-text"><strong>Retrieval-augmented generation (RAG)</strong> for knowledge-grounded responses</span>
      </div>
    </div>
  </div>
  
  <div class="tech-stack">
    <span class="tech-tag">Python</span>
    <span class="tech-tag">Transformers</span>
    <span class="tech-tag">LangChain</span>
    <span class="tech-tag">Vector Databases</span>
    <span class="tech-tag">FastAPI</span>
  </div>
  
  <div class="timeline-indicator">
    <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><rect x="3" y="4" width="18" height="18" rx="2"/><path d="M16 2v4M8 2v4M3 10h18"/></svg>
    Starting Soon
  </div>
</article>

</div>
