# Real-Time YouTube Comments Sentiment Analysis (GCP Data Engineering Pipeline)

**TL;DR (for recruiters):**  
This project demonstrates an **end-to-end real-time data engineering pipeline on Google Cloud Platform** that ingests YouTube comments, performs **sentiment analysis using NLP**, and serves analytics-ready data for dashboards. The system showcases production-oriented practices including **Infrastructure as Code (Terraform)**, **configuration automation (Ansible)**, **CI/CD with Jenkins**, **stream processing with Apache Beam / Dataflow**, **workflow orchestration with Airflow (Cloud Composer)**, and **analytics in BigQuery with Power BI visualization**.

---

## Project Overview

The goal of this project is to simulate a **production-style streaming data platform** capable of processing large volumes of real-time text data.

The pipeline collects **live YouTube comments**, analyzes their **sentiment (Positive, Neutral, Negative)**, and stores structured results in **BigQuery** for analytics and dashboarding.

This project demonstrates skills across **data engineering, cloud infrastructure, DevOps automation, and applied NLP**.

---

## Architecture

Pipeline workflow:

1. **YouTube API + Python**  
   A Python ingestion service retrieves YouTube comments and publishes them to Pub/Sub.

2. **Google Pub/Sub**  
   Serves as the real-time streaming ingestion layer.

3. **Apache Beam / Dataflow**  
   Processes incoming comments, applies sentiment analysis, and formats structured records.

4. **BigQuery**  
   Stores processed results and serves as the analytics warehouse.

5. **Cloud Composer (Airflow)**  
   Orchestrates pipelines, health checks, and workflow automation.

6. **Power BI**  
   Connects to BigQuery to provide dashboards and analytics.

7. **Terraform + Ansible + Jenkins**  
   Automates infrastructure provisioning, environment configuration, and CI/CD deployment.

---

## Tech Stack

**Cloud & Infrastructure**
- Google Cloud Platform
- Terraform (Infrastructure as Code)
- Ansible (Configuration management)

**Data Engineering**
- Pub/Sub (Streaming ingestion)
- Apache Beam / Dataflow (Stream processing)
- BigQuery (Data warehouse)

**Orchestration & Automation**
- Jenkins (CI/CD pipelines)
- Cloud Composer / Apache Airflow

**Programming**
- Python (ETL logic, API integration, NLP sentiment scoring)

**Visualization**
- Power BI

---

## Repository Structure
