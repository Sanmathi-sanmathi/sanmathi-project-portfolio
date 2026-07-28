# Fuel Tank Calibration Analysis

## What This Project Does

This solution uses Linear Regression to analyze fuel tank calibration data and generate a relationship between fuel level percentage and sensor voltage.

The tool automatically calculates calibration values, generates regression formulas, and visualizes the results using charts.

## Input

CSV file containing:

- Fuel Level (Liters)
- Sensor Voltage

## Processing

- Data cleaning
- Voltage correction
- Millivolt conversion
- Fuel percentage calculation
- Linear Regression modeling
- Calibration formula generation
- Visualization creation

## Output

- Calibrated dataset (.csv)
- Fuel Percentage vs Voltage formula
- Regression plots
- Tank capacity summary

## Sample Output

```text
Regression Formula

% = 0.0112 × MV + 3.7151
```

## Tech Stack

- Python
- Pandas
- NumPy
- Scikit-Learn
- Matplotlib

## Business Value

✅ Automates fuel tank calibration

✅ Generates calibration formulas

✅ Reduces manual calculations

✅ Supports fuel sensor validation

## Domain

Automotive Analytics | Fuel System Calibration

## Author

Sanmathi S