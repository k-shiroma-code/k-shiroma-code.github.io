---
title: Ongoing Projects
layout: default
permalink: /ongoing-projects/
description: A showcase of active development projects in data engineering, aerospace systems, and cybersecurity
---

<div style="text-align: center; margin-bottom: 30px;">
  <p>
    Welcome! This page highlights my <strong>in-progress projects</strong> — research and builds that are still being refined.  
    I’ll be publishing full GitHub repositories once the code and documentation are cleaned up.  
  </p>
</div>

---

## Enhanced Weather Data Pipeline with Apache Airflow <br><small>Started: June 2025 – Present</small>

A **production-grade data pipeline** for extracting, processing, and distributing weather data, built with **Apache Airflow** and modern data engineering best practices. The pipeline supports:  

- **Multi-source ingestion** (OpenWeather, WeatherAPI, AccuWeather, NOAA/NWS) with retry logic  
- **Data validation & schema evolution handling**  
- **Kubernetes-based scaling** for heavy workloads  
- **Monitoring & alerting** with Prometheus, Grafana, Slack, and PagerDuty  
- **Data lineage & audit logging** for compliance  

The modular DAG architecture enables **historical backfill, quality monitoring, and ML retraining**, making the system enterprise-ready for real-time analytics and forecasting.  

**Technologies:** Apache Airflow, Docker, MinIO, Kubernetes, Prometheus, Grafana, PostgreSQL, Delta Lake   

---

## Cybersecurity Research: IDS vs. Attack Traffic Generation <br><small>Started: July 2025 – Present</small>

This research explores the **contrasting but complementary roles** of intrusion detection systems (IDS) and active attack traffic generators. Using a **hybrid semi-supervised model** (Adaptive Support Vector Machine + Fuzzy C-Means), the IDS passively detects anomalies in real-time network traffic, while **T50** functions as an adversarial tool to generate high-volume, multi-protocol attack traffic.  

By combining the two, T50 becomes a **benchmarking framework** to stress-test IDS resilience and adaptability—creating a more **robust cybersecurity evaluation pipeline**.  

**Technologies:** Machine Learning (ASVM, FCM), Semi-supervised Learning, Network Security, T50 Traffic Generator  
**Reference:** [IEEE Xplore Digital Library ↗](https://ieeexplore.ieee.org/document/8058397/citations#citations)
