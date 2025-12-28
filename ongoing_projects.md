---
title: Ongoing Projects
layout: default
permalink: /ongoing-projects/
description: A showcase of active development projects!
---

## Weather API Project – Real-Time Forecasting and Time-Series Modeling

<p>
This project is a <strong>full-stack weather forecasting application</strong> that integrates <strong>real-time weather data</strong> with <strong>machine learning–based time-series forecasting</strong>. The system combines a <strong>FastAPI backend</strong>, an <strong>Astro and React frontend</strong>, and a <strong>SARIMA forecasting pipeline</strong> trained on <strong>five years of historical weather data</strong> for Tokyo.
</p>

<p>
The application provides <strong>current weather conditions for any city</strong> using the OpenWeather API and generates <strong>14-day temperature forecasts</strong> using a <strong>seasonal ARIMA model</strong>. The project emphasizes <strong>production-style architecture</strong>, <strong>data engineering workflows</strong>, and <strong>model interpretability</strong>.
</p>

<p>
<strong>Core Capabilities:</strong>
</p>

<ul>
  <li><strong>Real-time weather retrieval</strong> via REST API endpoints</li>
  <li><strong>14-day SARIMA-based temperature forecasts</strong></li>
  <li><strong>Interactive frontend dashboard</strong> with charts and tables</li>
  <li><strong>Automated ETL and ML training pipeline</strong></li>
  <li><strong>OpenAPI-documented backend</strong> using FastAPI</li>
</ul>

<p>
<strong>Machine Learning Details:</strong>
</p>

<ul>
  <li><strong>Model:</strong> SARIMA (Seasonal ARIMA) with yearly seasonality (365 days)</li>
  <li><strong>Training Data:</strong> ~5 years of daily weather data (2020–2024)</li>
  <li><strong>Forecast Horizon:</strong> 14 days</li>
  <li><strong>Evaluation Metrics:</strong> RMSE, MAE, MAPE</li>
</ul>

<p>
<strong>Technologies:</strong> Python, FastAPI, Astro, React, Pandas, NumPy, Statsmodels, Scikit-learn, Open-Meteo API, OpenWeather API
</p>

<p>
<a href="https://github.com/k-shiroma-code/Weather-API-Project" target="_blank" rel="noopener"><strong>View on GitHub ↗</strong></a>
</p>
