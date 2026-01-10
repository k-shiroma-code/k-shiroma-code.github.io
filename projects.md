---
title: Projects
layout: default
permalink: /projects/
---

## Weather & Energy Dashboard

A **full-stack web application** featuring **global weather data** and **California grid load forecasting** using machine learning. The dashboard predicts **14-day electricity demand** across **4 California service areas** (SCE, PG&E, SDG&E, VEA) using **Gradient Boosting, Random Forest, and Ridge Regression** models trained on **315,648 observations**. The best model achieved **2.26% MAPE** with **5-fold cross-validation**. The weather module provides **real-time forecasts** for any city worldwide with **°C/°F toggle** and **interactive charts**.

**Technologies:** React, Astro, FastAPI, Python, scikit-learn, Recharts, OpenWeather API  

<a href="https://github.com/k-shiroma-code/Weather-API-Project" target="_blank" rel="noopener"><strong>View on GitHub ↗</strong></a>

<div style="display: flex; gap: 10px; margin-top: 10px; flex-wrap: wrap;">
  <div style="flex: 1; min-width: 280px; background: linear-gradient(135deg, #1a1a2e 0%, #0f0f23 100%); border-radius: 8px; padding: 20px; border: 1px solid #333;">
    <h4 style="color: #f59e0b; margin-bottom: 10px;">📊 Model Performance</h4>
    <table style="width: 100%; font-size: 14px; color: #ccc;">
      <tr style="border-bottom: 1px solid #444;"><th style="text-align: left; padding: 5px 0;">Model</th><th>MAE</th><th>MAPE</th></tr>
      <tr><td>Gradient Boosting</td><td style="color: #10b981;">573 MW</td><td style="color: #10b981;">2.26%</td></tr>
      <tr><td>Random Forest</td><td>577 MW</td><td>2.29%</td></tr>
      <tr><td>Ridge + Weather</td><td>840 MW</td><td>3.41%</td></tr>
    </table>
  </div>
  <div style="flex: 1; min-width: 280px; background: linear-gradient(135deg, #1a1a2e 0%, #0f0f23 100%); border-radius: 8px; padding: 20px; border: 1px solid #333;">
    <h4 style="color: #f59e0b; margin-bottom: 10px;">🏢 Service Areas</h4>
    <ul style="font-size: 14px; color: #ccc; padding-left: 20px;">
      <li><strong>SCE</strong> – Southern California (15M people)</li>
      <li><strong>PG&E</strong> – Northern & Central CA (16M people)</li>
      <li><strong>SDG&E</strong> – San Diego Area (3.7M people)</li>
      <li><strong>VEA</strong> – Nevada/CA Border (45K people)</li>
    </ul>
  </div>
</div>

---

<div style="display: flex; gap: 24px; align-items: flex-start; flex-wrap: wrap;">

  <!-- Text content -->
  <div style="flex: 1; min-width: 300px;">
    <h2>EvoCharge – California EV Charging Cost Predictor</h2>

    <p>
      EvoCharge is a <strong>machine-learning dashboard</strong> that predicts electric vehicle charging
      energy usage and cost across California. The system uses
      <strong>3,500 charging sessions</strong>,
      <strong>16,455 statewide charging stations</strong>, and
      <strong>county-level electricity rates</strong> to power a
      <strong>real-time Lasso regression model</strong>.
    </p>

    <p>
      The app provides <strong>energy and cost estimates</strong>,
      an <strong>interactive station map</strong>, and
      <strong>detailed model insights</strong>.
      My contributions include <strong>designing the website in Figma</strong>
      and <strong>assisting with model testing and validation</strong>.
    </p>

    <p>
      <a href="https://evocharge.streamlit.app" target="_blank" rel="noopener"><strong>Live App ↗</strong></a> |
      <a href="https://github.com/anirudh9280/EvoCharge" target="_blank" rel="noopener"><strong>GitHub ↗</strong></a>
    </p>
  </div>

  <!-- Video -->
  <div style="flex: 1; min-width: 300px;">
    <video controls poster="{{ site.baseurl }}/assets/img/evocharge_screenshot.jpg"
      style="width: 100%; border-radius: 8px;">
      <source src="{{ site.baseurl }}/assets/img/EvoChargeDemo.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>

</div>

---

## Pulsepanion – AI Healthcare Tool (🏆 1st Place, 2025 Ai4Purpose Hackathon)

**Pulsepanion** is an **award-winning AI-based healthcare project** that analyzes eighteen months of patient data to generate **actionable insights for caregivers**. It applies **natural language processing (NLP)** with **large language models (LLMs)** via the **OpenAI API** and presents results in an **interactive R Shiny dashboard**. I also added a **PDF export feature** so caregivers can easily share summaries. The tool was designed to make it easier to identify patterns in patient data without manual review.  

**Technologies:** R Shiny, OpenAI API (LLM-based NLP), Healthcare Analytics  

<a href="https://github.com/k-shiroma-code/NCHacks-Pulsepanion" target="_blank" rel="noopener"><strong>View on GitHub ↗</strong></a>

<div style="display: flex; gap: 10px; margin-top: 10px;">
  <img src="{{ site.baseurl }}/assets/img/Pulsepantion.jpg" alt="Pulsepanion Dashboard" style="border-radius: 8px; width: 50%;">

  <div style="position: relative; padding-bottom: 28.125%; height: 0; width: 50%; border-radius: 8px; overflow: hidden; cursor: pointer;" onclick="this.style.position='fixed'; this.style.top='50%'; this.style.left='50%'; this.style.transform='translate(-50%, -50%)'; this.style.width='80vw'; this.style.height='80vh'; this.style.zIndex='9999'; this.style.paddingBottom='0'; this.style.backgroundColor='rgba(0,0,0,0.9)'; this.innerHTML='<iframe src=&quot;https://www.youtube.com/embed/tEJoXKLzVH4&quot; title=&quot;Pulsepanion Demo&quot; style=&quot;width:100%; height:100%; border:none;&quot; frameborder=&quot;0&quot; allowfullscreen></iframe><button onclick=&quot;event.stopPropagation(); this.parentElement.style.position=\&#39;relative\&#39;; this.parentElement.style.top=\&#39;auto\&#39;; this.parentElement.style.left=\&#39;auto\&#39;; this.parentElement.style.transform=\&#39;none\&#39;; this.parentElement.style.width=\&#39;50%\&#39;; this.parentElement.style.height=\&#39;0\&#39;; this.parentElement.style.zIndex=\&#39;auto\&#39;; this.parentElement.style.paddingBottom=\&#39;28.125%\&#39;; this.parentElement.style.backgroundColor=\&#39;transparent\&#39;; this.parentElement.innerHTML=\&#39;&lt;iframe src=\\&quot;https://www.youtube.com/embed/tEJoXKLzVH4\\&quot; title=\\&quot;Pulsepanion Demo\\&quot; style=\\&quot;position: absolute; top:0; left:0; width:100%; height:100%;\\&quot; frameborder=\\&quot;0\\&quot; allowfullscreen&gt;&lt;/iframe&gt;\&#39;&quot; style=&quot;position:absolute; top:10px; right:10px; background:rgba(255,255,255,0.8); border:none; border-radius:50%; width:30px; height:30px; cursor:pointer; font-size:16px;&quot;&gt;×</button>';">
    <iframe src="https://www.youtube.com/embed/tEJoXKLzVH4" title="Pulsepanion Demo" style="position: absolute; top:0; left:0; width:100%; height:100%;" frameborder="0" allowfullscreen></iframe>
  </div>
</div>

---

## Customer Segmentation Analytics

<div style="display: grid; grid-template-columns: 1fr 2fr; gap: 30px; margin: 20px 0; align-items: center;">
  <div style="min-width: 300px; max-width: 500px; display: flex; flex-direction: column; justify-content: center; height: 100%;">
    <p>
      This project delivers a <strong>comprehensive analysis of over 500,000 retail transactions</strong> to uncover <strong>behavioral patterns</strong> in customer activity. Using <strong>RFM (Recency, Frequency, Monetary) analysis</strong>, the study identified <strong>five distinct customer segments</strong>, revealed <strong>seasonal purchasing trends</strong>, and optimized <strong>marketing spend allocation by 25%</strong>. Developed with <strong>SQL, Tableau, and Python</strong>, the analytics pipeline converts raw sales data into <strong>clear insights for strategic business decisions</strong>.
    </p>
    <p>
      <strong>Technologies:</strong> SQL, Tableau, Python, RFM Analysis, Data Visualization<br>
      <a href="https://github.com/k-shiroma-code/Customer-Segmentation-with-RFM-Analysis" target="_blank" rel="noopener"><strong>View on GitHub ↗</strong></a>
    </p>
  </div>

  <div style="min-width: 400px; display: flex; justify-content: center; align-items: center;">
    <div style="width: 100%; aspect-ratio: 16/9; border-radius: 8px; overflow: hidden;">
      <iframe 
        src="https://public.tableau.com/views/Customer_Segmentation_Overview_Github/Dashboard1?:showVizHome=no&:embed=true" 
        style="width: 100%; height: 100%; border: none;">
      </iframe>
    </div>
  </div>
</div>

---

## Heart Disease Prediction Pipeline

This **machine learning pipeline** predicts **cardiovascular risk** using the **UCI Heart Disease dataset**. By addressing **class imbalance with SMOTE** and applying **logistic regression**, it achieved a **20% improvement in minority-class recall**. **Feature engineering and selection** ensured **optimal model performance**, and the final pipeline is designed for **production deployment** in healthcare analytics contexts.

**Technologies:** Python, Scikit-learn, SMOTE, Logistic Regression  
<a href="https://github.com/k-shiroma-code/Heart-Disease-ML-Project" target="_blank" rel="noopener"><strong>View on GitHub ↗</strong></a>

<div style="display: flex; gap: 10px; margin-top: 10px;">
  <img src="{{ site.baseurl }}/assets/img/IMG_1668.jpg" alt="Model Performance Metrics" style="border-radius: 8px; width: 50%;">
  <img src="{{ site.baseurl }}/assets/img/Feature_Importance.jpg" alt="Feature Importance Analysis" style="border-radius: 8px; width: 50%;">
</div>

---

## UEFA Euro 2024 Sports Analytics Project

This **sports analytics project** developed **predictive models** for UEFA Euro 2024 match outcomes by combining **ELO-based ratings** with traditional **statistical features**. Models such as **Decision Trees, Random Forests, and XGBoost** were trained and evaluated using **precision, recall, and F1-score** to identify the most effective approach.

The project also included **visualizations comparing predictions with actual outcomes**, providing insights into **model accuracy** and **forecasting reliability** in competitive sports analytics.

**Technologies:** Python, XGBoost, Feature Engineering, Statistical Modeling, Sports Analytics  
<a href="https://github.com/k-shiroma-code/CSUF-REU-Football-Analytics" target="_blank" rel="noopener"><strong>View on GitHub ↗</strong></a>

<div style="display: flex; gap: 10px; margin-top: 10px;">
  <img src="{{ site.baseurl }}/assets/img/IMG_1670.jpg" alt="UEFA Euro 2024 Prediction Visualization 1" style="border-radius: 8px; width: 50%;">
  <img src="{{ site.baseurl }}/assets/img/IMG_1671.jpg" alt="UEFA Euro 2024 Prediction Visualization 2" style="border-radius: 8px; width: 50%;">
</div>
