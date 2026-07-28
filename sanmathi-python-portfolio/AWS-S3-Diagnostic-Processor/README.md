# Vehicle Diagnostic Data Processing Pipeline

## What This Project Does

This solution automatically processes vehicle diagnostic scan logs stored in AWS S3 and converts raw XML files into structured datasets for analysis.

## Input

- Diagnostic Scan Log Files (XML)
- AWS S3 Storage

## Processing

- Download files from AWS S3
- Parse XML diagnostic logs
- Extract VIN and diagnostic information
- Calculate Active and Inactive DTC counts
- Classify ECU types
- Remove duplicate records
- Generate consolidated reports

## Output

- Processed Diagnostic Dataset (.csv)
- Analytics Dataset (.pkl)
- Error Logs (.txt / .json)

## Tech Stack

- Python
- AWS S3
- Boto3
- Pandas
- XML Processing

## Business Value

✅ Automates diagnostic log processing

✅ Reduces manual effort

✅ Improves data quality

✅ Generates analytics-ready datasets

## Domain

Automotive Diagnostics | Vehicle Telematics

## Author

Sanmathi S