# ETL Project: Scroll Points Analysis

## Overview
This project focuses on extracting wallet transaction data from the Scroll blockchain via Dune Analytics, transforming this data by fetching additional points information from an AWS API, and finally loading the cleaned and enriched data into Tableau for visualization and analysis.

## Process

### 1. Extract
- **Data Source**: Retrieved wallet addresses from Scroll blockchain transaction data using Dune Analytics.
- **API Endpoint**: Set up a custom API endpoint in Dune Analytics.
- **Data Retrieval**: Developed a Python script to fetch wallet data from the Dune API and save it into a CSV file.
- **Parallel Data Fetching**: Created an advanced Python script to fetch additional data in parallel requests from an AWS API using the wallet addresses from the CSV file, significantly speeding up the data retrieval process.

### 2. Transform
- **Data Cleaning**: Cleaned the fetched data to handle inconsistencies and errors.
- **Data Transformation**: Transformed the data by rounding numerical values, managing API rate limits, and ensuring all data was correctly formatted and complete.

### 3. Load
- **Data Storage**: Saved the final transformed data into a new CSV file.
- **Data Visualization**: Imported the cleaned and transformed data into Tableau to create insightful visualizations.

## Skills and Tools
- **PostgreSQL (Dune Analytics)**: Used for querying and extracting data from the Scroll blockchain.
- **Python**: Utilized to script the data extraction and transformation processes.
  - Libraries: `pandas`, `requests`, `concurrent.futures` for parallel processing.
- **API Integration and Management**: Expertise in handling API requests, managing rate limits, and error handling.
- **Data Cleaning and Transformation**: Ensured data accuracy and consistency through various cleaning and transformation techniques.
- **CSV File Handling**: Managed large datasets efficiently using CSV files.
- **Tableau**: Used to create visualizations to analyze and present the data.

## Scripts

#### Extracting Wallet Addresses from Dune API
#### Extracting Points from AWS API
