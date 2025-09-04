---
title: Ongoing Projects
layout: default
permalink: /ongoing-projects/
description: A showcase of active development projects in data engineering, aerospace systems, and cybersecurity
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

**Reference:** [IEEE Xplore Digital Library ↗](https://ieeexplore.ieee.org/document/8058397/)
