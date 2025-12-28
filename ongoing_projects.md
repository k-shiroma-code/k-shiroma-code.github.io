---
title: Ongoing Projects
layout: default
permalink: /ongoing-projects/
description: A showcase of active development projects!
---

## 🌤️ Weather API Project

**Status:** Actively Developing  
**Tech Focus:** Full-Stack Development · Machine Learning · Data Engineering

A full-stack weather forecasting application that combines **real-time weather data** with **AI-powered SARIMA temperature predictions**. The project demonstrates end-to-end development — from data ingestion and modeling to API design and frontend visualization.

---

### 🚀 Project Overview

This application provides:
- Real-time weather conditions for any city
- A 14-day temperature forecast powered by a SARIMA time-series model
- An interactive frontend dashboard with charts and tables
- A RESTful backend API built with FastAPI

The goal of this project is to showcase **production-style architecture**, **machine learning workflows**, and **clean API design**.

---

### 🏗️ Architecture

**Frontend**
- Astro + React
- Tailwind CSS
- Recharts for data visualization

**Backend**
- FastAPI REST API
- OpenWeather API for live data
- Model inference endpoints for ML forecasts

**Machine Learning Pipeline**
- Historical data from Open-Meteo (2020–2024)
- Automated ETL pipeline
- SARIMA model trained using `auto_arima`
- Evaluation with RMSE, MAE, and MAPE

---

### 🧠 Machine Learning Details

- **Model:** SARIMA (Seasonal ARIMA)
- **Seasonality:** 365 days
- **Training Data:** ~5 years of daily weather data (Tokyo)
- **Forecast Horizon:** 14 days
- **Features Used:**
  - Daily max temperature
  - Daily min temperature
  - Precipitation
  - Wind speed

This pipeline is fully reproducible and modular, allowing future expansion to additional locations or models.

---

### 🔌 API Capabilities

- `/weather?city=CityName`
- `/sarima/forecast?days=14`
- `/sarima/info`

Includes automatic OpenAPI documentation via FastAPI.

---

### 🛠️ Tech Stack

**Languages**
- Python
- JavaScript

**Frameworks & Libraries**
- FastAPI
- Astro
- React
- Pandas, NumPy
- Statsmodels
- Scikit-learn

**Data Sources**
- Open-Meteo API
- OpenWeather API

---

### 📍 Current Focus

- Improving forecast accuracy
- Expanding ML endpoints
- Enhancing frontend UX
- Preparing the project for cloud deployment

---

### 🔗 Links

- **GitHub Repository:**  
  https://github.com/k-shiroma-code/Weather-API-Project

- **API Docs (Local):**  
  http://localhost:8000/docs

---

_Last updated: December 2024_


