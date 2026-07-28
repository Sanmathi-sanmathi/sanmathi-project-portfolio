# OBU Transmission Validation Engine

## Overview

The OBU Transmission Validation Engine is a Python-based data validation
solution developed to analyze vehicle telematics data and verify OBU
(On-Board Unit) transmission intervals.

This tool calculates the forward time difference between consecutive OBU
timestamps, validates the expected 6-second transmission cycle, identifies
communication anomalies, and generates detailed output reports for further
analysis.

---

## Features

✅ OBU Timestamp Validation

✅ Forward Time Difference Calculation

✅ 6-Second Interval Verification

✅ Anomaly Detection and Classification

✅ Automated CSV Report Generation

✅ Full Dataset Export

✅ Anomalies-Only Export

✅ Large Dataset Processing Support

---

## Validation Logic

```text
Current OBU Timestamp
         │
         ▼
Next OBU Timestamp
         │
         ▼
Time Difference Calculation
         │
         ▼
Normal      = 6 Seconds
Anomaly     = Not 6 Seconds