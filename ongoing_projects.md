---
title: Ongoing Projects
layout: default
permalink: /ongoing-projects/
description: A showcase of active development projects in data engineering, machine learning, and cybersecurity
---
<div style="text-align: center; margin-bottom: 30px;">
  <p>
    Welcome! This page highlights my <strong>in-progress projects</strong> — research and builds that are still being refined.  
    I'll be publishing full GitHub repositories once the code and documentation are cleaned up.  
  </p>
</div>

---

## Weather Data Pipeline with Apache Airflow
**Started: June 2025 – Present**

A **data pipeline project** for collecting and processing weather data using **Apache Airflow** and Python. The system demonstrates core data engineering concepts including:

- **API data extraction** from OpenWeatherMap with error handling and rate limiting
- **Data cleaning and transformation** using pandas with validation checks  
- **Scheduled data collection** running daily via Airflow DAGs
- **Database storage** in PostgreSQL with proper schema design and indexing
- **Monitoring and notifications** using Airflow's built-in UI and email alerts
- **Data visualization** with Python libraries (matplotlib/plotly) for weather trend analysis

The pipeline collects weather data for multiple cities, handles missing values and API failures, and stores historical records for time-series analysis. Includes comprehensive **unit tests, documentation, and version control** following software development best practices.

**Technologies:** Apache Airflow, Python, pandas, Apache Spark (exploring), PostgreSQL, Docker, Git, REST APIs

**Key Learning Outcomes:**
- Workflow orchestration and scheduling
- API integration with robust error handling
- Database design and SQL operations
- Data quality validation techniques
- Containerization with Docker

---

## Medical Image Classification with Deep Learning
**Started: September 2025 – Present**

A **computer vision project** exploring transfer learning techniques for medical image analysis. This educational research project demonstrates responsible AI development in healthcare contexts by building a skin lesion classification system using pre-trained convolutional neural networks.

**Project Focus:**
- **Transfer learning implementation** using EfficientNet/ResNet architectures
- **Data preprocessing pipeline** with image augmentation and normalization
- **Model evaluation** with medical-relevant metrics (sensitivity, specificity, AUROC)
- **Interpretability tools** including Grad-CAM visualization for model decisions
- **Ethical AI practices** with proper data handling and bias consideration
- **Web deployment** using Streamlit for interactive demonstrations

The system performs binary classification on dermatological images while emphasizing the educational nature of the project. Includes comprehensive documentation on model architecture decisions, evaluation methodologies, and responsible AI principles in healthcare applications.

**Technologies:** Python, TensorFlow/Keras, OpenCV, scikit-learn, Streamlit, Matplotlib, NumPy

**Key Learning Outcomes:**
- Transfer learning with pre-trained CNN models
- Medical image preprocessing techniques
- Model interpretability and explainability methods
- Responsible AI development practices
- Healthcare data handling considerations

**Note:** *This project is for educational and research purposes only and is not intended for medical diagnosis. Always consult qualified healthcare professionals for medical concerns.*

---

## Cybersecurity Research: IDS Performance Evaluation Framework
**Started: July 2025 – Present**

This research project develops a **comprehensive evaluation framework** for testing intrusion detection systems (IDS) against various attack patterns. The project implements a **hybrid semi-supervised learning model** combining Adaptive Support Vector Machines (ASVM) with Fuzzy C-Means clustering to detect network anomalies in real-time traffic.

The framework uses **T50 traffic generator** to create controlled attack scenarios for systematic IDS testing, enabling performance benchmarking across different attack types and network conditions. This creates a **standardized testing environment** for comparing IDS effectiveness and identifying areas for improvement.

**Technologies:** Python, Machine Learning (ASVM, FCM), Network Security, T50 Traffic Generator, Wireshark, Linux

**Research Focus:**
- Semi-supervised anomaly detection algorithms
- Network traffic analysis and pattern recognition
- IDS performance metrics and evaluation methodologies
- Attack simulation and traffic generation

**Note:** *This is a long-term research project that will likely extend into and form the foundation for a Master's thesis in cybersecurity or machine learning.*

**Reference:** [IEEE Xplore Digital Library ↗](https://ieeexplore.ieee.org/document/8058397/)
