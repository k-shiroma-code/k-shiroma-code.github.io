---
title: Ongoing Projects
layout: default
permalink: /ongoing-projects/
description: A showcase of active development projects!
---

## **Weather API Project**

**Status:** **Actively Developing**  
**Focus Areas:** **Full-Stack Development**, **Machine Learning**, **Data Engineering**

A **full-stack weather forecasting application** that combines **real-time weather data** with **machine learning–based time-series forecasting**. This project demonstrates **end-to-end system design**, from data ingestion and model training to API development and frontend visualization.

---

### **Project Overview**

The **Weather API Project** delivers:

- **Real-time weather conditions** for any city  
- **14-day temperature forecasts** using a **SARIMA time-series model**  
- An **interactive web dashboard** with charts and tables  
- A **RESTful backend API** built with **FastAPI**

The project is designed to reflect **production-style architecture** and practical machine learning workflows.

---

### **System Architecture**

**Frontend**
- **Astro** and **React**
- **Tailwind CSS**
- **Recharts** for data visualization

**Backend**
- **FastAPI** REST API
- **OpenWeather API** for live weather data
- Dedicated endpoints for **machine learning inference**

**Machine Learning Pipeline**
- **Historical data** from the **Open-Meteo API** (2020–2024)
- Automated **ETL pipeline**
- **SARIMA model** trained using `auto_arima`
- Evaluation using **RMSE**, **MAE**, and **MAPE**

---

### **Machine Learning Details**

- **Model:** **SARIMA (Seasonal ARIMA)**
- **Seasonality:** **365 days**
- **Training Data:** Approximately **five years** of daily weather data (Tokyo)
- **Forecast Horizon:** **14 days**
- **Features Used:**
  - Daily maximum temperature  
  - Daily minimum temperature  
  - Daily precipitation  
  - Maximum wind speed  

The pipeline is **modular and reproducible**, allowing future expansion to additional locations or alternative forecasting models.

---

### **API Capabilities**

- **GET `/weather?city=CityName`**  
- **GET `/sarima/forecast?days=14`**  
- **GET `/sarima/info`**

The backend includes **automatically generated OpenAPI documentation** via FastAPI.

---

### **Technology Stack**

**Languages**
- **Python**
- **JavaScript**

**Frameworks and Libraries**
- **FastAPI**
- **Astro**
- **React**
- **Pandas**
- **NumPy**
- **Statsmodels**
- **Scikit-learn**

**Data Sources**
- **Open-Meteo API**
- **OpenWeather API**

---

### **Current Development Focus**

- Improving **forecast accuracy** and model stability  
- Expanding **machine learning endpoints**  
- Enhancing **frontend usability and performance**  
- Preparing the application for **cloud deployment**

---

### **Live Project and Source Code**

- **Live Project Page:**  
  **https://k-shiroma-code.github.io/Weather-API-Project/**

- **GitHub Repository:**  
  **https://github.com/k-shiroma-code/Weather-API-Project**

---

**Last updated:** **December 2024**
## **Weather API Project**

**Status:** **Actively Developing**  
**Focus Areas:** **Full-Stack Development**, **Machine Learning**, **Data Engineering**

A **full-stack weather forecasting application** that combines **real-time weather data** with **machine learning–based time-series forecasting**. This project demonstrates **end-to-end system design**, from data ingestion and model training to API development and frontend visualization.

---

### **Project Overview**

The **Weather API Project** delivers:

- **Real-time weather conditions** for any city  
- **14-day temperature forecasts** using a **SARIMA time-series model**  
- An **interactive web dashboard** with charts and tables  
- A **RESTful backend API** built with **FastAPI**

The project is designed to reflect **production-style architecture** and practical machine learning workflows.

---

### **System Architecture**

**Frontend**
- **Astro** and **React**
- **Tailwind CSS**
- **Recharts** for data visualization

**Backend**
- **FastAPI** REST API
- **OpenWeather API** for live weather data
- Dedicated endpoints for **machine learning inference**

**Machine Learning Pipeline**
- **Historical data** from the **Open-Meteo API** (2020–2024)
- Automated **ETL pipeline**
- **SARIMA model** trained using `auto_arima`
- Evaluation using **RMSE**, **MAE**, and **MAPE**

---

### **Machine Learning Details**

- **Model:** **SARIMA (Seasonal ARIMA)**
- **Seasonality:** **365 days**
- **Training Data:** Approximately **five years** of daily weather data (Tokyo)
- **Forecast Horizon:** **14 days**
- **Features Used:**
  - Daily maximum temperature  
  - Daily minimum temperature  
  - Daily precipitation  
  - Maximum wind speed  

The pipeline is **modular and reproducible**, allowing future expansion to additional locations or alternative forecasting models.

---

### **API Capabilities**

- **GET `/weather?city=CityName`**  
- **GET `/sarima/forecast?days=14`**  
- **GET `/sarima/info`**

The backend includes **automatically generated OpenAPI documentation** via FastAPI.

---

### **Technology Stack**

**Languages**
- **Python**
- **JavaScript**

**Frameworks and Libraries**
- **FastAPI**
- **Astro**
- **React**
- **Pandas**
- **NumPy**
- **Statsmodels**
- **Scikit-learn**

**Data Sources**
- **Open-Meteo API**
- **OpenWeather API**

---

### **Current Development Focus**

- Improving **forecast accuracy** and model stability  
- Expanding **machine learning endpoints**  
- Enhancing **frontend usability and performance**  
- Preparing the application for **cloud deployment**

---

### **Live Project and Source Code**

- **Live Project Page:**  
  **https://k-shiroma-code.github.io/Weather-API-Project/**

- **GitHub Repository:**  
  **https://github.com/k-shiroma-code/Weather-API-Project**

---

