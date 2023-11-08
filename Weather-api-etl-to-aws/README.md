# Weather Data ETL Pipeline with Airflow

This repository contains an Apache Airflow DAG (Directed Acyclic Graph) for extracting weather data from an API, transforming it, and loading it into a CSV file on Amazon S3. The DAG performs the following steps:

1. **Check API Availability:** It starts by checking the availability of the weather data API.
2. **Extract Weather Data:** If the API is available, it extracts weather data for a specific city (e.g., Houston) from the API.
3. **Transform and Load Data:** After extracting the data, it transforms the raw JSON response into a structured format and loads it into a CSV file stored on Amazon S3.

## DAG Structure

The DAG consists of three main tasks:

1. **is_weather_api_ready:** This task checks the availability of the weather data API.

2. **extract_weather_data:** It extracts the raw weather data from the API.

3. **transform_load_weather_data:** This task transforms the raw data and loads it into an S3 bucket.

## Prerequisites

Before using this DAG, make sure you have the following:

- Apache Airflow installed and configured.
- API credentials for the weather data source.
- AWS S3 credentials for uploading data.

## Usage

1. Clone this repository:

   ```bash
   git clone <repository_url>
