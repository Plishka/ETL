# ETL Project: Scroll Points Analysis

## Overview
This project involved extracting wallet transaction data from Scroll blockchain using Dune Analytics, transforming the data by fetching additional points information from an external API, and loading the cleaned data into Tableau for visualization.

## Process

### 1. Extract
- Retrieved wallet transaction data from Dune Analytics.
- Saved the data into a CSV file.

### 2. Transform
- Used wallet addresses from the CSV to query an external API for additional points data.
- Cleaned and transformed the data, including rounding numerical values and handling API rate limits and errors.

### 3. Load
- Saved the final transformed data into a new CSV file.
- Imported the CSV into Tableau for creating interactive dashboards and visualizations.

## Skills and Tools
- Python (pandas, requests)
- API integration and management
- Data cleaning and transformation
- CSV file handling
- Tableau for data visualization

