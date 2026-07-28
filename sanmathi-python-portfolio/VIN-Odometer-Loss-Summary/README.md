# VIN Odometer Loss Summary

## What This Project Does

This tool analyzes vehicle odometer data and identifies odometer loss for each VIN.

Users can select a folder containing multiple vehicle CSV files, and the tool automatically calculates the total odometer loss and displays the results in a user-friendly interface.

## Input

CSV files containing:

- VIN
- Event Time
- Odometer

## Processing

- Read all CSV files from a selected folder
- Sort records by Event Time
- Calculate odometer differences
- Identify odometer loss values
- Generate VIN-wise summary

## Output

Summary table containing:

```text
VIN
Overall Odometer Loss (Km)
```

Option to export results as CSV.

## Features

✅ Folder-Based Processing

✅ VIN-Wise Analysis

✅ Odometer Loss Calculation

✅ Summary Report Generation

✅ CSV Export

✅ Interactive GUI

## Tech Stack

- Python
- Pandas
- Tkinter

## Business Value

✅ Identifies odometer anomalies

✅ Reduces manual analysis effort

✅ Supports data quality validation

✅ Enables quick vehicle-level analysis

## Domain

Vehicle Telematics | Data Validation | Odometer Analytics

## Author

Sanmathi S