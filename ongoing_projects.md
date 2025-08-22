---
title: Ongoing Projects
layout: default
permalink: /ongoing*projects/
description: A showcase of active development projects in data engineering, aerospace systems, and cybersecurity
---

<div class="hero-section" style="background: linear-gradient(135deg, #667eea 0%, #764ba2 100%); color: white; padding: 60px 20px; text-align: center; margin-bottom: 40px; border-radius: 10px;">
  <h1 style="font-size: 3em; margin-bottom: 20px; text-shadow: 2px 2px 4px rgba(0,0,0,0.3);">🚀 Ongoing Projects</h1>
  <p style="font-size: 1.3em; opacity: 0.9; max-width: 800px; margin: 0 auto;">
    Welcome to my collection of active development projects! Each project represents a deep dive into cutting-edge technologies and practical applications of data engineering, aerospace systems, and cybersecurity.
  </p>
</div>

<div class="projects-container" style="max-width: 1200px; margin: 0 auto; padding: 0 20px;">

<!-- Weather Data Pipeline Project -->
<div class="project-card" style="background: #f8f9fa; border-radius: 15px; padding: 40px; margin-bottom: 40px; box-shadow: 0 10px 30px rgba(0,0,0,0.1); border-left: 5px solid #4CAF50;">
  <div class="project-header" style="display: flex; align-items: center; margin-bottom: 25px; flex-wrap: wrap;">
    <h2 style="color: #2c3e50; margin: 0; flex: 1;">🌤️ Weather Data Pipeline with Apache Airflow</h2>
    <div class="project-badges" style="display: flex; gap: 10px; flex-wrap: wrap;">
      <span style="background: #28a745; color: white; padding: 5px 12px; border-radius: 20px; font-size: 0.85em; font-weight: bold;">Active Development</span>
      <span style="background: #17a2b8; color: white; padding: 5px 12px; border-radius: 20px; font-size: 0.85em;">Data Engineering</span>
    </div>
  </div>
  
  <div class="project-meta" style="margin-bottom: 20px;">
    <strong>Tech Stack:</strong> 
    <code style="background: #e9ecef; padding: 2px 6px; border-radius: 4px; margin: 0 3px;">Apache Airflow</code>
    <code style="background: #e9ecef; padding: 2px 6px; border-radius: 4px; margin: 0 3px;">Docker</code>
    <code style="background: #e9ecef; padding: 2px 6px; border-radius: 4px; margin: 0 3px;">MinIO</code>
    <code style="background: #e9ecef; padding: 2px 6px; border-radius: 4px; margin: 0 3px;">Python</code>
    <code style="background: #e9ecef; padding: 2px 6px; border-radius: 4px; margin: 0 3px;">Prometheus</code>
  </div>

  <p style="font-size: 1.1em; line-height: 1.6; color: #495057; margin-bottom: 25px;">
    A comprehensive, enterprise-grade data pipeline that extracts, processes, and stores weather data from multiple APIs. Built with scalability, reliability, and monitoring as core principles.
  </p>

  <div class="features-grid" style="display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 20px; margin-bottom: 25px;">
    <div style="background: white; padding: 20px; border-radius: 8px; border-left: 3px solid #4CAF50;">
      <strong>🔄 Multi-source Integration</strong><br>
      <small style="color: #6c757d;">OpenWeatherMap, WeatherAPI, and NOAA data sources with automatic failover</small>
    </div>
    <div style="background: white; padding: 20px; border-radius: 8px; border-left: 3px solid #2196F3;">
      <strong>📊 Real-time Monitoring</strong><br>
      <small style="color: #6c757d;">Prometheus metrics with Grafana dashboards and intelligent alerting</small>
    </div>
    <div style="background: white; padding: 20px; border-radius: 8px; border-left: 3px solid #FF9800;">
      <strong>🛡️ Data Quality Validation</strong><br>
      <small style="color: #6c757d;">Weather-specific validation rules and automated quality scoring</small>
    </div>
    <div style="background: white; padding: 20px; border-radius: 8px; border-left: 3px solid #9C27B0;">
      <strong>🚀 Scalable Processing</strong><br>
      <small style="color: #6c757d;">Containerized tasks with Kubernetes Pod Operator support</small>
    </div>
  </div>

  <div class="architecture-section" style="background: white; padding: 20px; border-radius: 8px; margin-bottom: 25px;">
    <h4 style="color: #2c3e50; margin-bottom: 15px;">🏗️ System Architecture</h4>
    <div style="font-family: 'Courier New', monospace; background: #f8f9fa; padding: 15px; border-radius: 5px; overflow-x: auto;">
Weather APIs → Airflow DAGs → MinIO Storage → Analytics<br>
     ↓              ↓             ↓           ↓<br>
  Validation → Processing → Monitoring → Alerts
    </div>
  </div>

  <div class="progress-section" style="margin-bottom: 25px;">
    <h4 style="color: #2c3e50; margin-bottom: 15px;">🎯 Current Progress</h4>
    <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 15px;">
      <div>
        <strong style="color: #28a745;">✅ Completed</strong>
        <ul style="margin: 8px 0; padding-left: 20px; color: #495057;">
          <li>Core pipeline implementation</li>
          <li>Multi-source API integration</li>
          <li>MinIO object storage</li>
          <li>Monitoring and alerting</li>
        </ul>
      </div>
      <div>
        <strong style="color: #ffc107;">🔄 In Progress</strong>
        <ul style="margin: 8px 0; padding-left: 20px; color: #495057;">
          <li>ML weather prediction models</li>
          <li>Real-time streaming ingestion</li>
          <li>Advanced pattern analysis</li>
        </ul>
      </div>
    </div>
  </div>

  <div class="project-links" style="display: flex; gap: 15px; flex-wrap: wrap;">
    <a href="#" style="background: #007bff; color: white; padding: 10px 20px; border-radius: 25px; text-decoration: none; font-weight: bold; transition: all 0.3s;">🔗 View Repository</a>
    <a href="#" style="background: #28a745; color: white; padding: 10px 20px; border-radius: 25px; text-decoration: none; font-weight: bold; transition: all 0.3s;">📊 Live Dashboard</a>
    <a href="#" style="background: #17a2b8; color: white; padding: 10px 20px; border-radius: 25px; text-decoration: none; font-weight: bold; transition: all 0.3s;">📖 Documentation</a>
  </div>
</div>

<!-- Telemetry Data Rocketry Project -->
<div class="project-card" style="background: #f8f9fa; border-radius: 15px; padding: 40px; margin-bottom: 40px; box-shadow: 0 10px 30px rgba(0,0,0,0.1); border-left: 5px solid #FF6B35;">
  <div class="project-header" style="display: flex; align-items: center; margin-bottom: 25px; flex-wrap: wrap;">
    <h2 style="color: #2c3e50; margin: 0; flex: 1;">🚀 Telemetry Data Rocketry System</h2>
    <div class="project-badges" style="display: flex; gap: 10px; flex-wrap: wrap;">
      <span style="background: #FF6B35; color: white; padding: 5px 12px; border-radius: 20px; font-size: 0.85em; font-weight: bold;">Active Development</span>
      <span style="background: #6f42c1; color: white; padding: 5px 12px; border-radius: 20px; font-size: 0.85em;">Aerospace</span>
    </div>
  </div>
  
  <div class="project-meta" style="margin-bottom: 20px;">
    <strong>Tech Stack:</strong> 
    <code style="background: #e9ecef; padding: 2px 6px; border-radius: 4px; margin: 0 3px;">Python</code>
    <code style="background: #e9ecef; padding: 2px 6px; border-radius: 4px; margin: 0 3px;">InfluxDB</code>
    <code style="background: #e9ecef; padding: 2px 6px; border-radius: 4px; margin: 0 3px;">Grafana</code>
    <code style="background: #e9ecef; padding: 2px 6px; border-radius: 4px; margin: 0 3px;">Arduino</code>
    <code style="background: #e9ecef; padding: 2px 6px; border-radius: 4px; margin: 0 3px;">LoRa</code>
  </div>

  <p style="font-size: 1.1em; line-height: 1.6; color: #495057; margin-bottom: 25px;">
    <strong>Collaboration with Norco Rocketry Club:</strong> Analyzing real hotfire telemetry data using advanced time series techniques to identify patterns, detect anomalies, and develop forecasting models. This project demonstrates expertise in time series preprocessing, exploratory data analysis, classical and deep learning modeling, and anomaly detection for aerospace applications.
  </p>

  <div class="features-grid" style="display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 20px; margin-bottom: 25px;">
    <div style="background: white; padding: 20px; border-radius: 8px; border-left: 3px solid #FF6B35;">
      <strong>📈 Time Series Analysis</strong><br>
      <small style="color: #6c757d;">Advanced preprocessing, trend analysis, and seasonality decomposition</small>
    </div>
    <div style="background: white; padding: 20px; border-radius: 8px; border-left: 3px solid #3F51B5;">
      <strong>🔍 Anomaly Detection</strong><br>
      <small style="color: #6c757d;">Statistical and ML-based methods for identifying system irregularities</small>
    </div>
    <div style="background: white; padding: 20px; border-radius: 8px; border-left: 3px solid #4CAF50;">
      <strong>🎯 Forecasting Models</strong><br>
      <small style="color: #6c757d;">ARIMA, LSTM, and ensemble methods for predictive analytics</small>
    </div>
    <div style="background: white; padding: 20px; border-radius: 8px; border-left: 3px solid #E91E63;">
      <strong>🚀 Hotfire Analysis</strong><br>
      <small style="color: #6c757d;">Specialized rocket engine testing data interpretation and visualization</small>
    </div>
  </div>

  <div class="data-structure-section" style="background: white; padding: 25px; border-radius: 8px; margin-bottom: 25px; border: 1px solid #e9ecef;">
    <h4 style="color: #2c3e50; margin-bottom: 15px;">📊 Dataset Structure</h4>
    <div style="background: #f8f9fa; padding: 15px; border-radius: 5px; font-family: 'Courier New', monospace; margin-bottom: 15px;">
      <strong>Raw CSV Format:</strong><br>
      • <code>timestamp</code>: Date and time of measurement<br>
      • <code>sensor_id</code>: Identifier for sensor/device<br>
      • <code>value</code>: Measured reading (temperature, pressure, voltage)<br>
      • <code>location</code>: Physical sensor location<br>
      • <code>status_flag</code>: System health indicators
    </div>
    <p style="color: #495057; margin: 0;">
      <strong>Analysis Objectives:</strong> Explore trends and seasonality, detect abnormal system behavior, and forecast future values using both statistical and machine learning approaches.
    </p>
  </div>

  <div class="progress-section" style="margin-bottom: 25px;">
    <h4 style="color: #2c3e50; margin-bottom: 15px;">🎯 Analysis Progress</h4>
    <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 15px;">
      <div>
        <strong style="color: #28a745;">✅ Data Processing Complete</strong>
        <ul style="margin: 8px 0; padding-left: 20px; color: #495057;">
          <li>CSV data cleaning and preprocessing</li>
          <li>Exploratory data analysis (EDA)</li>
          <li>Trend and seasonality decomposition</li>
          <li>Statistical anomaly identification</li>
        </ul>
      </div>
      <div>
        <strong style="color: #ffc107;">🔄 Model Development</strong>
        <ul style="margin: 8px 0; padding-left: 20px; color: #495057;">
          <li>Classical time series models (ARIMA)</li>
          <li>Deep learning approaches (LSTM)</li>
          <li>Ensemble forecasting methods</li>
          <li>Real-time anomaly detection systems</li>
        </ul>
      </div>
    </div>
  </div>

  <div class="project-links" style="display: flex; gap: 15px; flex-wrap: wrap;">
    <a href="#" style="background: #FF6B35; color: white; padding: 10px 20px; border-radius: 25px; text-decoration: none; font-weight: bold; transition: all 0.3s;">🔗 View Repository</a>
    <a href="#" style="background: #6f42c1; color: white; padding: 10px 20px; border-radius: 25px; text-decoration: none; font-weight: bold; transition: all 0.3s;">📊 Analysis Results</a>
    <a href="#" style="background: #17a2b8; color: white; padding: 10px 20px; border-radius: 25px; text-decoration: none; font-weight: bold; transition: all 0.3s;">🚀 Norco Collaboration</a>
  </div>
</div>

<!-- Cybersecurity ML Project -->
<div class="project-card" style="background: #f8f9fa; border-radius: 15px; padding: 40px; margin-bottom: 40px; box-shadow: 0 10px 30px rgba(0,0,0,0.1); border-left: 5px solid #DC3545;">
  <div class="project-header" style="display: flex; align-items: center; margin-bottom: 25px; flex-wrap: wrap;">
    <h2 style="color: #2c3e50; margin: 0; flex: 1;">🛡️ Cybersecurity ML Intrusion Detection</h2>
    <div class="project-badges" style="display: flex; gap: 10px; flex-wrap: wrap;">
      <span style="background: #DC3545; color: white; padding: 5px 12px; border-radius: 20px; font-size: 0.85em; font-weight: bold;">Experimental</span>
      <span style="background: #6c757d; color: white; padding: 5px 12px; border-radius: 20px; font-size: 0.85em;">Cybersecurity</span>
    </div>
  </div>
  
  <div class="project-meta" style="margin-bottom: 20px;">
    <strong>Tech Stack:</strong> 
    <code style="background: #e9ecef; padding: 2px 6px; border-radius: 4px; margin: 0 3px;">Python</code>
    <code style="background: #e9ecef; padding: 2px 6px; border-radius: 4px; margin: 0 3px;">TensorFlow</code>
    <code style="background: #e9ecef; padding: 2px 6px; border-radius: 4px; margin: 0 3px;">Scikit-learn</code>
    <code style="background: #e9ecef; padding: 2px 6px; border-radius: 4px; margin: 0 3px;">Wireshark</code>
    <code style="background: #e9ecef; padding: 2px 6px; border-radius: 4px; margin: 0 3px;">Elastic Stack</code>
  </div>

  <p style="font-size: 1.1em; line-height: 1.6; color: #495057; margin-bottom: 25px;">
    <strong>Research Focus:</strong> IDS vs. Attack Traffic Generation - A comprehensive study exploring the symbiotic relationship between defensive AI systems (hybrid ASVM + FCM models) and controlled offensive testing tools (T50 traffic generator). This research demonstrates how adversarial testing validates and improves AI-driven security systems.
  </p>

  <div class="thesis-section" style="background: #fff3cd; padding: 20px; border-radius: 8px; margin-bottom: 25px; border-left: 4px solid #ffc107;">
    <h4 style="color: #856404; margin-bottom: 15px;">📋 Thesis Statement</h4>
    <p style="color: #856404; font-style: italic; line-height: 1.6;">
      While <strong>intrusion detection systems</strong> (IDS) such as hybrid semi-supervised <strong>ASVM</strong> (Adaptive Support Vector Machine) and <strong>FCM</strong> (Fuzzy C-Means) models provide passive and adaptive defense mechanisms, tools like <strong>T50</strong> operate as active stress-testing frameworks that generate high-volume, multi-protocol attack traffic. Their contrasting roles reveal a <strong>complementary relationship</strong> for strengthening network security evaluation.
    </p>
  </div>

  <div class="dual-approach-section" style="display: grid; grid-template-columns: 1fr 1fr; gap: 30px; margin-bottom: 25px;">
    <div style="background: white; padding: 25px; border-radius: 12px; border: 2px solid #28a745;">
      <h4 style="color: #155724; margin-bottom: 15px;">🛡️ Defensive Side: Hybrid IDS Model</h4>
      <ul style="list-style: none; padding: 0; color: #495057;">
        <li style="margin-bottom: 8px;">🎯 <strong>ASVM</strong>: Adaptive Support Vector Machine for classification</li>
        <li style="margin-bottom: 8px;">🧠 <strong>FCM</strong>: Fuzzy C-Means for clustering anomalies</li>
        <li style="margin-bottom: 8px;">📚 <strong>Semi-supervised learning</strong>: Adapts to new attack patterns</li>
        <li>👁️ <strong>Passive monitoring</strong>: Real-time traffic analysis</li>
      </ul>
    </div>
    <div style="background: white; padding: 25px; border-radius: 12px; border: 2px solid #dc3545;">
      <h4 style="color: #721c24; margin-bottom: 15px;">⚔️ Offensive Side: T50 Traffic Generator</h4>
      <ul style="list-style: none; padding: 0; color: #495057;">
        <li style="margin-bottom: 8px;">🌐 <strong>Multi-protocol support</strong>: Various attack vectors</li>
        <li style="margin-bottom: 8px;">⚡ <strong>High-volume traffic</strong>: Stress tests system capacity</li>
        <li style="margin-bottom: 8px;">🔬 <strong>Controlled environment</strong>: Ethical penetration testing</li>
        <li>📊 <strong>Benchmark tool</strong>: Standardized attack simulation</li>
      </ul>
    </div>
  </div>

  <div class="experiments-section" style="background: white; padding: 20px; border-radius: 8px; margin-bottom: 25px;">
    <h4 style="color: #2c3e50; margin-bottom: 15px;">🧪 Current Experiments</h4>
    <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); gap: 20px;">
      <div style="border-left: 3px solid #007bff; padding-left: 15px;">
        <strong>Adversarial ML Defense</strong><br>
        <small style="color: #6c757d;">Testing model robustness against adversarial attacks and evasion techniques</small>
      </div>
      <div style="border-left: 3px solid #28a745; padding-left: 15px;">
        <strong>Federated Learning</strong><br>
        <small style="color: #6c757d;">Distributed training across multiple network segments without data sharing</small>
      </div>
      <div style="border-left: 3px solid #ffc107; padding-left: 15px;">
        <strong>Graph Neural Networks</strong><br>
        <small style="color: #6c757d;">Network topology analysis for advanced persistent threat detection</small>
      </div>
      <div style="border-left: 3px solid #dc3545; padding-left: 15px;">
        <strong>Explainable AI</strong><br>
        <small style="color: #6c757d;">Interpretable models for security analyst decision support</small>
      </div>
    </div>
  </div>

  <div class="metrics-section" style="background: #fff3cd; padding: 20px; border-radius: 8px; margin-bottom: 25px; border: 1px solid #ffeaa7;">
    <h4 style="color: #856404; margin-bottom: 15px;">📈 Performance Metrics (Latest Experiments)</h4>
    <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(150px, 1fr)); gap: 15px; text-align: center;">
      <div>
        <strong style="font-size: 1.8em; color: #28a745;">94.7%</strong><br>
        <small style="color: #856404;">Detection Rate</small>
      </div>
      <div>
        <strong style="font-size: 1.8em; color: #007bff;">0.3%</strong><br>
        <small style="color: #856404;">False Positive Rate</small>
      </div>
      <div>
        <strong style="font-size: 1.8em; color: #6f42c1;">125ms</strong><br>
        <small style="color: #856404;">Avg Response Time</small>
      </div>
      <div>
        <strong style="font-size: 1.8em; color: #fd7e14;">12</strong><br>
        <small style="color: #856404;">Attack Types Detected</small>
      </div>
    </div>
  </div>

  <div class="progress-section" style="margin-bottom: 25px;">
    <h4 style="color: #2c3e50; margin-bottom: 15px;">🎯 Research Progress</h4>
    <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 15px;">
      <div>
        <strong style="color: #28a745;">✅ Foundation Complete</strong>
        <ul style="margin: 8px 0; padding-left: 20px; color: #495057;">
          <li>Baseline ML models implemented</li>
          <li>Dataset collection and preprocessing</li>
          <li>Real-time data pipeline</li>
        </ul>
      </div>
      <div>
        <strong style="color: #ffc107;">🔬 Active Research</strong>
        <ul style="margin: 8px 0; padding-left: 20px; color: #495057;">
          <li>Advanced neural architectures</li>
          <li>Adversarial robustness testing</li>
          <li>Model interpretability improvements</li>
        </ul>
      </div>
    </div>
  </div>

  <div class="project-links" style="display: flex; gap: 15px; flex-wrap: wrap;">
    <a href="#" style="background: #DC3545; color: white; padding: 10px 20px; border-radius: 25px; text-decoration: none; font-weight: bold; transition: all 0.3s;">🔗 View Repository</a>
    <a href="#" style="background: #6c757d; color: white; padding: 10px 20px; border-radius: 25px; text-decoration: none; font-weight: bold; transition: all 0.3s;">📊 Experiment Results</a>
    <a href="https://ieeexplore.ieee.org/document/8058397/citations#citations" style="background: #007bff; color: white; padding: 10px 20px; border-radius: 25px; text-decoration: none; font-weight: bold; transition: all 0.3s;">📄 IEEE Reference</a>
  </div>
</div>

</div>

<!-- Footer Section -->
<div class="footer-section" style="background: #2c3e50; color: white; padding: 40px 20px; text-align: center; border-radius: 10px; margin-top: 60px;">
  <h3 style="margin-bottom: 20px;">🤝 Collaboration & Contact</h3>
  <p style="font-size: 1.1em; opacity: 0.9; margin-bottom: 25px; max-width: 600px; margin-left: auto; margin-right: auto;">
    Interested in collaborating on any of these projects? I'm always open to discussions, contributions, and knowledge sharing in data engineering, aerospace systems, and cybersecurity research.
  </p>
  <div style="display: flex; justify-content: center; gap: 20px; flex-wrap: wrap;">
    <a href="mailto:your-email@example.com" style="background: #3498db; color: white; padding: 10px 20px; border-radius: 25px; text-decoration: none; font-weight: bold;">✉️ Email</a>
    <a href="https://github.com/yourusername" style="background: #333; color: white; padding: 10px 20px; border-radius: 25px; text-decoration: none; font-weight: bold;">🔗 GitHub</a>
    <a href="https://linkedin.com/in/yourprofile" style="background: #0077b5; color: white; padding: 10px 20px; border-radius: 25px; text-decoration: none; font-weight: bold;">💼 LinkedIn</a>
  </div>
</div>

<style>
/* Responsive design improvements */
@media (max-width: 768px) {
  .hero-section h1 {
    font-size: 2em !important;
  }
  .project-header {
    flex-direction: column !important;
    align-items: flex-start !important;
  }
  .project-header h2 {
    margin-bottom: 10px !important;
  }
  .features-grid {
    grid-template-columns: 1fr !important;
  }
}

/* Hover effects for links */
.project-links a:hover {
  transform: translateY(-2px);
  box-shadow: 0 5px 15px rgba(0,0,0,0.2);
}

/* Animation for project cards */
.project-card {
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.project-card:hover {
  transform: translateY(-5px);
  box-shadow: 0 15px 40px rgba(0,0,0,0.15) !important;
}
</style>
