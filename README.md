# Real-Time YouTube Comments Sentiment Analysis (GCP Data Engineering Pipeline)

## Project Overview

The goal of this project is to simulate a **production-style streaming data platform** capable of processing large volumes of real-time text data.

The pipeline collects **live YouTube comments**, analyzes their **sentiment (Positive, Neutral, Negative)**, and stores structured results in **BigQuery** for analytics and dashboarding via PowerBI.

This project demonstrates skills across **data engineering + DevOps + AI**.

---

## Architecture

<p align="center">
  <img width="100%" src="docs/architecture.jpg" alt="Project Architecture">
</p>

Pipeline workflow:

1. **YouTube API + Python** → A Python ingestion service retrieves YouTube comments and publishes them to Pub/Sub.

2. **Google Pub/Sub** → Serves as the real-time streaming ingestion layer.

3. **Apache Beam / Dataflow** → Processes incoming comments, applies sentiment analysis, and formats structured records.

4. **BigQuery** → Stores processed results and serves as the analytics warehouse.

5. **Cloud Composer (Airflow)** → Orchestrates pipelines, health checks, and workflow automation.

6. **Power BI** → Connects to BigQuery to provide dashboards and analytics.

7. **Terraform + Ansible + Jenkins** →  Automates infrastructure provisioning, environment configuration, and CI/CD deployment.

---


## Repository Structure

