# Retail-Store-Data-processing-using-DataBricks

Retail Store Data processing using DataBricks and AWS Services

This project demonstrates a real-time data processing pipeline leveraging AWS services to ingest, process, and store streaming data efficiently for analytics and reporting.

Overview

The pipeline processes streaming data from Amazon Kinesis Data Streams, performs transformation and staging using AWS Lambda, orchestrates workflow using Apache Airflow, and stores the data in a Delta Lake format via AWS EMR. The processed data is made available for querying through Amazon Athena, enabling real-time business insights.

Architecture Components
	•	Amazon Kinesis Data Streams: Captures real-time streaming data.
	•	AWS Lambda (Archive Layer): Reads data from Kinesis and stores the raw stream into an S3 archive layer.
	•	AWS Lambda (Transformation Layer): Flattens nested JSON data and performs micro-batching before storing to the S3 stage layer.
	•	Apache Airflow: Manages and schedules the data pipeline workflow.
	•	Task 1: Triggers pipeline execution with staged data.
	•	Task 2: Uses AWS EMR to create a raw layer and ingests transformed data into Delta Lake tables.
	•	Amazon Athena: Enables querying of the data stored in Delta Lake for business analytics.

Key Features
	•	Serverless ingestion and transformation using AWS Lambda.
	•	Real-time data streaming and storage.
	•	Modular and scalable architecture using Apache Airflow and AWS EMR.
	•	Queryable Delta Lake storage for cost-effective, on-demand analytics.

Technologies Used
	•	AWS Lambda
	•	Amazon Kinesis
	•	Amazon S3
	•	Apache Airflow
	•	AWS EMR
	•	Delta Lake
	•	Amazon Athena
