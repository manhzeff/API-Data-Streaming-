This project serves as a comprehensive guide to building an end-to-end data engineering pipeline. It covers each stage from data ingestion to processing and finally to storage, utilizing a robust tech stack that includes Apache Airflow, Python, Apache Kafka, Apache Zookeeper, Apache Spark, and Cassandra. Everything is containerized using Docker for ease of deployment and scalability.

**The workflow of the project**
![image](https://github.com/manhzeff/API-Data-Streaming-/assets/104782892/b93dbf38-4008-4f4c-a56e-3d4ec2c731b3)

The project is designed with the following components:

# Project Overview

This project leverages a variety of technologies to establish a robust data pipeline. Below is an outline of the key components and their roles within the system.

## Data Source

- **Random User Generator**: We utilize the [randomuser.me](https://randomuser.me/) API to generate random user data, which serves as the initial input for our pipeline.

## Data Orchestration

- **Apache Airflow**: Orchestrates the pipeline, managing the workflow from data ingestion to storage. Airflow is responsible for fetching data from the Random User Generator API and storing it in a PostgreSQL database.

## Data Streaming

- **Apache Kafka and Zookeeper**: Facilitate the streaming of data from the PostgreSQL database to our processing engine. Kafka, in conjunction with Zookeeper, ensures reliable and scalable streaming capabilities.

## Monitoring and Schema Management

- **Control Center and Schema Registry**: Essential for the monitoring and management of Kafka streams. The Control Center provides a comprehensive overview of the system's health and performance, while the Schema Registry maintains the integrity of data schemas within our streams.

## Data Processing

- **Apache Spark**: Employs both master and worker nodes to process the data efficiently. Apache Spark's robust computing capabilities enable complex data transformations and analyses.

## Data Storage

- **Cassandra**: The final destination for our processed data. Cassandra's distributed architecture ensures scalability and reliability for storing large volumes of data.

