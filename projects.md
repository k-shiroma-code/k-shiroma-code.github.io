---
title: Projects
layout: default
permalink: /projects/
---

## Pulsepanion – AI Healthcare Tool

### Pulsepanion  
**Pulsepanion** is an **AI-based healthcare project** that takes about eighteen months of patient data and turns it into **useful insights for caregivers**. It uses **natural language processing (NLP)** to process the records and provides an **interactive R Shiny dashboard** where users can explore results. I also added a **PDF export feature** so caregivers can easily share summaries. The goal was to make it easier to find patterns and insights in patient data without having to go through everything manually.  

**Technologies:** R Shiny, OpenAI API, NLP, Healthcare Analytics  

<a href="https://github.com/k-shiroma-code/NCHacks-Pulsepanion">View on GitHub ↗</a>

<div style="display: flex; gap: 10px; margin-top: 10px;">
  <!-- Image -->
  <img src="{{ site.baseurl }}/assets/img/Pulsepantion.jpg" alt="Pulsepanion Dashboard" style="border-radius: 8px; width: 50%;">

  <!-- Video -->
  <div style="position: relative; padding-bottom: 28.125%; height: 0; width: 50%; border-radius: 8px; overflow: hidden; cursor: pointer;" onclick="this.style.position='fixed'; this.style.top='50%'; this.style.left='50%'; this.style.transform='translate(-50%, -50%)'; this.style.width='80vw'; this.style.height='80vh'; this.style.zIndex='9999'; this.style.paddingBottom='0'; this.style.backgroundColor='rgba(0,0,0,0.9)'; this.innerHTML='<iframe src=&quot;https://www.youtube.com/embed/tEJoXKLzVH4&quot; title=&quot;Pulsepanion Demo&quot; style=&quot;width:100%; height:100%; border:none;&quot; frameborder=&quot;0&quot; allowfullscreen></iframe><button onclick=&quot;event.stopPropagation(); this.parentElement.style.position=\&#39;relative\&#39;; this.parentElement.style.top=\&#39;auto\&#39;; this.parentElement.style.left=\&#39;auto\&#39;; this.parentElement.style.transform=\&#39;none\&#39;; this.parentElement.style.width=\&#39;50%\&#39;; this.parentElement.style.height=\&#39;0\&#39;; this.parentElement.style.zIndex=\&#39;auto\&#39;; this.parentElement.style.paddingBottom=\&#39;28.125%\&#39;; this.parentElement.style.backgroundColor=\&#39;transparent\&#39;; this.parentElement.innerHTML=\&#39;&lt;iframe src=\\&quot;https://www.youtube.com/embed/tEJoXKLzVH4\\&quot; title=\\&quot;Pulsepanion Demo\\&quot; style=\\&quot;position: absolute; top:0; left:0; width:100%; height:100%;\\&quot; frameborder=\\&quot;0\\&quot; allowfullscreen&gt;&lt;/iframe&gt;\&#39;&quot; style=&quot;position:absolute; top:10px; right:10px; background:rgba(255,255,255,0.8); border:none; border-radius:50%; width:30px; height:30px; cursor:pointer; font-size:16px;&quot;&gt;×</button>';">
    <iframe src="https://www.youtube.com/embed/tEJoXKLzVH4" title="Pulsepanion Demo" style="position: absolute; top:0; left:0; width:100%; height:100%;" frameborder="0" allowfullscreen></iframe>
  </div>
</div>

---

## Customer Segmentation Analytics

<div style="display: grid; grid-template-columns: 1fr 2fr; gap: 30px; margin: 20px 0; align-items: center;">

  <!-- Text column -->
  <div style="min-width: 300px; max-width: 500px; display: flex; flex-direction: column; justify-content: center; height: 100%;">
    <p>
      This project delivers a <strong>comprehensive analysis of over 500,000 retail transactions</strong> to uncover <strong>behavioral patterns</strong> in customer activity. Using <strong>RFM (Recency, Frequency, Monetary) analysis</strong>, the study identified <strong>five distinct customer segments</strong>, revealed <strong>seasonal purchasing trends</strong>, and optimized <strong>marketing spend allocation by 25%</strong>. Developed with <strong>SQL, Tableau, and Python</strong>, the analytics pipeline converts raw sales data into <strong>clear insights for strategic business decisions</strong>.
    </p>
    <p>
      <strong>Technologies:</strong> SQL, Tableau, Python, RFM Analysis, Data Visualization<br>
      <a href="https://github.com/k-shiroma-code/Customer-Segmentation-with-RFM-Analysis">View on GitHub ↗</a>
    </p>
  </div>

  <!-- Dashboard column -->
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

<p>This <strong>machine learning pipeline</strong> predicts <strong>cardiovascular risk</strong> using the <strong>UCI Heart Disease dataset</strong>. By addressing <strong>class imbalance with SMOTE</strong> and applying <strong>logistic regression</strong>, it achieved a <strong>20% improvement in minority-class recall</strong>. <strong>Feature engineering and selection</strong> ensured <strong>optimal model performance</strong>, and the final pipeline is designed for <strong>production deployment</strong> in healthcare analytics contexts.</p>
<p><strong>Technologies:</strong> Python, Scikit-learn, SMOTE, Logistic Regression<br>
<a href="https://github.com/k-shiroma-code/Heart-Disease-ML-Project" target="_blank" rel="noopener">View on GitHub ↗</a>

<div style="display: flex; gap: 10px; margin-top: 10px;">
  <img src="{{ site.baseurl }}/assets/img/IMG_1668.jpg" alt="Model Performance Metrics" style="border-radius: 8px; width: 50%;">
  <img src="{{ site.baseurl }}/assets/img/Feature_Importance.jpg" alt="Feature Importance Analysis" style="border-radius: 8px; width: 50%;">
</div>

---

## CSUF Data Science Project – UEFA Euro 2024 Match Prediction

<div class="project-card">
  <h3 class="project-title">UEFA Euro 2024 Sports Analytics Project</h3>
  <p class="project-description">
    This <strong>sports analytics project</strong> developed <strong>predictive models</strong> for UEFA Euro 2024 match outcomes by combining <strong>ELO-based ratings</strong> with traditional <strong>statistical features</strong>. Models such as <strong>Decision Trees, Random Forests, and XGBoost</strong> were trained and evaluated using <strong>precision, recall, and F1-score</strong> to identify the most effective approach.
  </p>
  <p class="project-description">
    The project also included <strong>visualizations comparing predictions with actual outcomes</strong>, providing insights into <strong>model accuracy</strong> and <strong>forecasting reliability</strong> in competitive sports analytics.
  </p>
  <p class="project-tech">
    <strong>Technologies:</strong> Python, XGBoost, Feature Engineering, Statistical Modeling, Sports Analytics
  </p>
  <a href="https://github.com/k-shiroma-code/CSUF-REU-Football-Analytics" class="project-link" target="_blank">View on GitHub ↗</a>
</div>

<div style="display: flex; gap: 10px; margin-top: 10px;">
  <img src="{{ site.baseurl }}/assets/img/IMG_1670.jpg" alt="UEFA Euro 2024 Prediction Visualization 1" style="border-radius: 8px; width: 50%;">
  <img src="{{ site.baseurl }}/assets/img/IMG_1671.jpg" alt="UEFA Euro 2024 Prediction Visualization 2" style="border-radius: 8px; width: 50%;">
</div>

---
