# YouTube Trending Data Analysis Pipeline

## Overview
This project focuses on building a **secure and scalable data pipeline** to ingest, process, and analyze structured and semi-structured data related to **YouTube trending videos**. The system processes data from multiple regions and performs analytics based on **video categories and trending metrics** such as views, likes, comments, and engagement patterns.

The architecture leverages **cloud-based data engineering services** to handle large datasets efficiently and enable insightful reporting through interactive dashboards.

---

## Project Goals

### 1. Data Ingestion
Design a mechanism to **collect and ingest data from multiple sources** and load it into a centralized storage system.

### 2. ETL Pipeline
The raw dataset requires transformation before analysis. The ETL pipeline performs:
- Data extraction from source files
- Data transformation into structured formats
- Data loading into a data lake for further processing

### 3. Data Lake Architecture
Since the project collects data from multiple regions and files, a **centralized storage repository** is required to store raw and processed datasets efficiently.

### 4. Scalability
The system is designed to **scale with increasing data volumes**, ensuring efficient processing and storage as new data is continuously added.

### 5. Cloud Infrastructure
Processing large datasets locally is inefficient. Therefore, this project uses **cloud computing infrastructure** to manage and process data at scale.

### 6. Reporting and Visualization
Build interactive dashboards to answer analytical questions such as:
- Which video categories trend the most?
- Which regions generate the highest engagement?
- What factors influence trending videos?

---

## AWS Services Used

### Amazon S3
Amazon S3 is used as the **data lake storage layer**. It provides scalable object storage with high availability, security, and durability.

### AWS IAM
AWS Identity and Access Management (IAM) is used to securely manage access and permissions for AWS resources.

### AWS Glue
AWS Glue is a **serverless ETL service** used to discover, transform, and catalog data for analytics.

### AWS Lambda
AWS Lambda is used to run **event-driven serverless functions** without managing infrastructure.

### AWS Athena
AWS Athena allows users to run **interactive SQL queries directly on data stored in Amazon S3** without loading it into a database.

### Amazon QuickSight
Amazon QuickSight is used to build **interactive dashboards and visualizations** for analyzing the data.

---

## Dataset

This project uses the **YouTube Trending Dataset**, which contains statistics on daily trending YouTube videos across multiple regions.

The dataset includes:
- Video title
- Channel title
- Publication time
- Tags
- Views
- Likes and dislikes
- Comment count
- Video description

Each region's dataset is stored in separate CSV files, and a JSON file provides **category mappings** using the `category_id` field.

Dataset Source:  
https://www.kaggle.com/datasets/datasnaek/youtube-new

---

## Key Outcomes
- Built a **cloud-based data pipeline**
- Implemented **ETL workflows for data transformation**
- Stored and processed large datasets in a **scalable data lake**
- Enabled **serverless analytics using AWS services**
- Created **interactive dashboards for insights and reporting**
