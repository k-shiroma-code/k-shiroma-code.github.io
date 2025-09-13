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


