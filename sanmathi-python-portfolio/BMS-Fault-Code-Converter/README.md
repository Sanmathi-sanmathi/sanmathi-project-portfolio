# BMS Fault Code Converter

## What This Project Does

This tool extracts BMS Fault Codes from the `fault_status_4` parameter and generates a processed CSV file with decoded fault information.

Users can select an input CSV file, process the data, and save the output through a simple desktop interface.

## Input

CSV file containing:

```text
fault_status_4
```

## Processing

- Read input CSV
- Extract second byte from fault_status_4
- Convert to BMS Fault Code
- Create processed output file

## Output

CSV file containing:

```text
BMS Fault Code
```

along with the original data.

## Features

✅ Automatic Fault Code Extraction

✅ CSV Processing

✅ Output File Generation

✅ User-Friendly GUI

✅ Error Handling

✅ Multi-Threaded Processing

## Tech Stack

- Python
- Pandas
- Tkinter

## Business Value

✅ Eliminates manual fault code conversion

✅ Reduces engineering effort

✅ Improves analysis efficiency

✅ Supports diagnostics validation

## Domain

Automotive Diagnostics | Data Processing | Automation

## Author

Sanmathi S