# Vehicle Data Retrieval Tool

## What This Project Does

This tool provides a simple desktop interface to retrieve vehicle data from an API using Asset IDs and VINs.

Users can upload a list of vehicles, select a message type and date range, and automatically download vehicle data into CSV files.

## Input

- Asset ID List
- VIN List
- Message Type
- Start Date
- End Date

## Processing

- Read Asset IDs and VINs from CSV
- Fetch data from API
- Handle pagination automatically
- Sort records by Event Time
- Generate VIN-wise output files

## Output

```text
VIN_1.csv
VIN_2.csv
VIN_3.csv
...
```

Each file contains vehicle data for the selected period.

## Features

✅ CSV Upload

✅ Date Range Selection

✅ Message Type Selection

✅ Automated API Data Retrieval

✅ VIN-wise CSV Generation

✅ Progress Tracking

✅ User-Friendly GUI

## Tech Stack

- Python
- Tkinter
- Requests
- Pandas
- CSV

## Business Value

✅ Eliminates manual API queries

✅ Saves engineering effort

✅ Faster vehicle data extraction

✅ Easy bulk data download

## Domain

Vehicle Telematics | API Automation

## Author

Sanmathi S
