# DTLA Parameter Converter

## What This Project Does

This tool converts DTLA status values into meaningful parameter fields by decoding binary data from a CSV file.

Users can upload a CSV file, process the DTLA status column, and generate an output file with additional decoded parameters.

## Input

CSV file containing:

```text
dtlastatus
```

## Processing

- Read input CSV
- Convert DTLA status to binary
- Extract parameter values
- Generate decoded status fields
- Save transformed data to CSV

## Output

CSV file containing:

```text
DTLA Solenoid

MOR Switch Status

SOR Switch Status

Traction Switch
```

## Features

✅ CSV File Processing

✅ Binary Data Decoding

✅ Automated Parameter Extraction

✅ Output CSV Generation

✅ Progress Tracking

✅ User-Friendly GUI

## Tech Stack

- Python
- Pandas
- Tkinter

## Business Value

✅ Eliminates manual binary decoding

✅ Improves analysis efficiency

✅ Reduces human errors

✅ Accelerates vehicle diagnostics review

## Domain

Vehicle Diagnostics | Data Processing | Automation

## Author

Sanmathi S
