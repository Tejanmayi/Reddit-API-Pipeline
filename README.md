# 🚀 Reddit ETL Pipeline for r/dataengineering

A robust and end-to-end data pipeline that extracts Reddit data from [r/dataengineering](https://www.reddit.com/r/dataengineering/) and transforms it into insightful analytics on Google Data Studio.

## 📌 Overview

This project was inspired by a deep interest in the data engineering domain and the valuable discussions on its official subreddit. It serves as a hands-on learning experience across several data tools and platforms including:

- **Reddit API**
- **AWS (S3 + Redshift)**
- **dbt**
- **Apache Airflow**
- **Docker**
- **Terraform**
- **Google Data Studio / Power BI**

The project may be over-engineered for a small dataset, but it's designed to mirror real-world data engineering architectures.

---

## 🧑‍💻 Architecture

![Workflow](https://github.com/ABZ-Aaron/Reddit-API-Pipeline/blob/master/images/workflow.png)

### 🔁 Pipeline Steps

1. **Extract**: Pull posts using the [Reddit API](https://www.reddit.com/dev/api/)
2. **Load**: Store raw data in [AWS S3](https://aws.amazon.com/s3/)
3. **Warehouse**: Load data into [AWS Redshift](https://aws.amazon.com/redshift/)
4. **Transform**: Clean & model data with [dbt](https://www.getdbt.com/)
5. **Visualize**: Build interactive dashboards in [Google Data Studio](https://datastudio.google.com) or [Power BI](https://powerbi.microsoft.com/)
6. **Orchestrate**: Automate with [Apache Airflow](https://airflow.apache.org) inside [Docker](https://www.docker.com/)
7. **Infrastructure as Code**: Manage resources via [Terraform](https://www.terraform.io/)

---

---

## ⚙️ Setup Instructions

You can recreate this project end-to-end by following the instructions below.

> **Important**: This setup was developed on an M1 MacBook Pro. Minor tweaks might be required if you're using Windows or Linux.

> **Disclaimer**: AWS Free Tier should cover most services used here, but always double-check the latest [Free Tier limits](https://aws.amazon.com/free/) before deploying.

### 🔧 Installation

```bash
git clone https://github.com/ABZ-Aaron/Reddit-API-Pipeline.git
cd Reddit-API-Pipeline
```

### 📁 Setup Guide

1. [Project Overview](instructions/overview.md)  
2. [Reddit API Configuration](instructions/reddit.md)  
3. [Create AWS Account](instructions/aws.md)  
4. [Provision Infrastructure with Terraform](instructions/setup_infrastructure.md)  
5. [Configuration Details](instructions/config.md)  
6. [Run Airflow in Docker](instructions/docker_airflow.md)  
7. [Setup dbt Models](instructions/dbt.md)  
8. [Build the Dashboard](instructions/visualisation.md)  
9. [Terminate Resources](instructions/terminate.md)  
10. [Future Improvements](instructions/improvements.md)  

---

## ✅ Features

- Extracts real Reddit threads and metadata
- Scalable and modular ETL pipeline
- Cleaned and structured data using dbt
- Automated orchestration using Airflow
- Easy deployment with Terraform
- Beautiful dashboards for storytelling

---

## 📌 Improvements Planned

- Add sentiment analysis for posts and comments
- Schedule daily incremental data loads
- Integrate with a message queue (Kafka)
- Switch from static CSV to live dashboard using APIs or streaming data

---

## 👨‍💻 Author

**Tejanmayi**  
📧 [LinkedIn](https://linkedin.com/in/your-link) • 🧠 [Portfolio](https://your-portfolio.com)  
This project was built for educational purposes and portfolio demonstration.