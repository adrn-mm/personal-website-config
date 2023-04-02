---
title: "Data Engineering 101"
date: 2023-04-01
slug: data-engineering-101
tags: ["Data Engineering"]
summary: An introduction and key concepts to data engineering. It's a concise overview for anyone seeking a basic understanding of data engineering.
weight: 1
description: An introduction and key concepts to data engineering. It's a concise overview for anyone seeking a basic understanding of data engineering.
cover: 
  image: 
  alt: 
  caption: 
  relative: true
draft: false
---

## Who is Data Engineer?
- Data engineer is someone who builds a data-driven system so that data can be easily utilized by a company.
- We need data engineers because the data is scattered in many places, still raw, and too big. Data engineers are responsible for collecting, processing, and storing data so that it can be used by data scientists and analysts.
- The tasks of data engineer:
  - Designing and monitoring the architecture of Data Platform and Pipeline
  - Integrating data from multiple sources into a single source (Data Ingestion)
  - Implementing **Data Governance**. Data governance is the process of managing and controlling data within a company (Data Quality, Data Security & Privacy, Data Access Management).
  - Implementing **Data Lifecycle Management**
    - Data Collection & Processing
    - Data Storage
    - Data Use & Analysis
    - Data Deletion

## Data Pipeline
- Pipeline Components
  - Sources
  - Staging/Landing
  - Data Warehouse
  - Data Mart
- ETL
  - ![](https://learn.microsoft.com/id-id/azure/architecture/data-guide/images/etl.png)
- ELT
  - ![](https://learn.microsoft.com/id-id/azure/architecture/data-guide/images/elt.png)
  - Advantages:
    - Flexibility data formats
    - Tranformation as needed
    - Speed of Loading
  - Disadvantages:
    - Not suitable for non-cloud users
    - Sensitive data may not comply with regulation
    - Lower speed of analysis

## Data Ingestion
- Data ingestion is a process of transporting data from one or more sources to a target site.
- Stream
- Batch
- Lambda Architecture
	![](https://hazelcast.com/wp-content/uploads/2021/12/19_Lambda-1.png)

## OLTP vs. OLAP
- Online Transaction Processing
- Online Analytical Processing
![](https://forum.huawei.com/enterprise/en/data/attachment/forum/202110/11/201214j8t9ixu3t7epm0to.jpg)

## Data Lake, Data Warehouse, & Data Mart
1. Data Lake focus is on storing raw and unstructured data from various sources in a storage location, in unstructured or semi-structured formats like files, images, or streaming data, at a low cost, and providing fast access to the data.
1. Data Warehouse focus is on creating a centralized storage location for data taken from various sources and organized in a way that can be used for analysis. Data in the data warehouse is transformed into a structured format and arranged in a star or snowflake schema, with the aim of supporting decision-making and business analysis.
2. Data marts are a subset of the data warehouse that focus on a specific business area, such as sales or finance. They are taken from the data warehouse and presented in a format suitable for business purposes. Data marts are used to meet the specific needs of departments or for specific business analysis needs.

## Relational and Non-Relational Databases
- Relational databases consist of tables with rows and columns, which are related to each other using primary and foreign keys. The data is organized using a schema, and SQL (Structured Query Language) is used to interact with the database. Relational databases are suitable for applications that require high data integrity and complex transactions, and tools like MySQL, MS SQL Server, and PostgreSQL are commonly used.
- Non-relational databases, also known as NoSQL, use a more flexible data model, such as document, graph, or key-value store, and are not organized in a fixed schema. They are suitable for applications that require horizontal scalability and the ability to manage unstructured data. Tools like MongoDB, Cassandra, and Redis are commonly used for NoSQL databases.
![](https://thorntech-com-media-cloud.s3.amazonaws.com/2022/03/SQLvsNoSQL.jpg)