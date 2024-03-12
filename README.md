This project serves as a comprehensive guide to building an end-to-end data engineering pipeline. It covers each stage from data ingestion to processing and finally to storage, utilizing a robust tech stack that includes Apache Airflow, Python, Apache Kafka, Apache Zookeeper, Apache Spark, and Cassandra. Everything is containerized using Docker for ease of deployment and scalability.

**The workflow of the project**
![image](https://github.com/manhzeff/API-Data-Streaming-/assets/104782892/b93dbf38-4008-4f4c-a56e-3d4ec2c731b3)

The project is designed with the following components:

1.Data Source: We use randomuser.me API to generate random user data for our pipeline.
2.Apache Airflow: Responsible for orchestrating the pipeline and storing fetched data in a PostgreSQL database.
3.Apache Kafka and Zookeeper: Used for streaming data from PostgreSQL to the processing engine.
4.Control Center and Schema Registry: Helps in monitoring and schema management of our Kafka streams.
5.Apache Spark: For data processing with its master and worker nodes.
6.Cassandra: Where the processed data will be stored.
