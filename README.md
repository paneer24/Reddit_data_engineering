## Data Pipeline with Reddit, Airflow, Celery, Postgres, S3, AWS Glue, Athena, and Redshift.

This project provides a comprehensive data pipeline solution to extract, transform, and load (ETL) Reddit data into a Redshift data warehouse. The pipeline leverages a combination of tools and services including Apache Airflow, Celery, PostgreSQL, Amazon S3, AWS Glue, Amazon Athena, and Amazon Redshift.

## Table of Contents
- Overview
- Architecture

## Overview
The pipeline is designed to:

1. Extract data from Reddit using its API.
2. Store the raw data into an S3 bucket from Airflow.
3. Transform the data using AWS Glue and Amazon Athena.
4. Load the transformed data into Amazon Redshift for analytics and querying.

## Architecture
[![image](https://github.com/user-attachments/assets/7905be6f-991f-4760-9e9f-44c71e8489e0)](https://github.com/airscholar/RedditDataEngineering/raw/main/assets%2FRedditDataEngineering.png)

1. Reddit API: Source of the data.
2. Apache Airflow & Celery: Orchestrates the ETL process and manages task distribution.
3. PostgreSQL: Temporary storage and metadata management.
4. Amazon S3: Raw data storage.
5. AWS Glue: Data cataloging and ETL jobs.
6. Amazon Athena: SQL-based data transformation.
7. Amazon Redshift: Data warehousing and analytics.
