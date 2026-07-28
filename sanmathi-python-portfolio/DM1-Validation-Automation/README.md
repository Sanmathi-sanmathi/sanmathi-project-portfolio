# DM1 Fault Validation & Qualification Engine

## Project Overview

This solution automates the validation of incoming DM1 fault records by comparing them against a master fault database.

Instead of manually reviewing hundreds or thousands of fault records, the tool automatically analyzes each DM1 entry and determines whether the fault is qualified, partially matched, or requires further investigation.

The final output provides clear qualification status and mismatch reasons for every record.

---

## Business Problem

Engineering and diagnostics teams often receive DM1 fault data from vehicle telematics systems.

Manually verifying every fault against a master fault database is:

- Time consuming
- Error prone
- Difficult to scale for large datasets

This automation eliminates manual comparison and generates validation results within seconds.

---

## Input Data

### File 1: Master Database

Contains approved fault records.

Example:

```text
SPN_FMI | Source Address | Description        | Pcode
------------------------------------------------------
1234    | 0              | Engine Over Speed | P001
5678    | 1              | Oil Pressure Low  | P002
```

### File 2: Incoming DM1 Data

Contains telematics fault records that need validation.

Example:

```text
SPN_FMI | Source Address | Description        | Pcode
------------------------------------------------------
1234    | 0              | Engine Over Speed | P001
5678    | 1              | Oil Pressure High | P002
```

---

## Validation Process

```text
Incoming DM1 Record
          │
          ▼
Compare With Master Database
          │
          ▼
Validate Source Address
          │
          ▼
Validate SPN/FMI
          │
          ▼
Validate Description
          │
          ▼
Validate Pcode
          │
          ▼
Generate Qualification Result
```

---

## Qualification Rules

### Qualified

All fields match.

```text
SPN_FMI        ✅
Source Address ✅
Description    ✅
Pcode          ✅
```

Result:

```text
Qualified
```

---

### Source Address Mismatch

Fault details match but Source Address differs.

Result:

```text
Not Feasible

Reason:
Source Address Mismatch
```

---

### Pcode Mismatch

SPN_FMI and Description match but Pcode differs.

Result:

```text
Not Feasible

Reason:
Pcode Mismatch
```

---

### Description Mismatch

SPN_FMI and Pcode match but Description differs.

Result:

```text
Not Feasible

Reason:
Description Mismatch
```

---

### Unique Fault

No matching record exists in master database.

Result:

```text
Not Feasible

Reason:
Unique Fault Record
```

---

## Output

The tool automatically generates a CSV report.

### Output Columns

```text
VEE Status

VEE Description

Master Data Description

VEE Remarks
```

---

## Sample Output

```text
VEE Status : Qualified

VEE Remarks : Exact Match
```

```text
VEE Status : Not Feasible

VEE Remarks : Source Address Mismatch
```

```text
VEE Status : Not Feasible

VEE Remarks : Only Pcode Matches
```

---

## Key Features

- Automated DM1 Validation
- Master Database Comparison
- Source Address Verification
- SPN/FMI Validation
- Description Validation
- Pcode Validation
- Mismatch Detection
- Qualification Status Generation
- Automated CSV Report Creation
- Large Dataset Processing

---

## Business Value

✅ Eliminates manual fault verification

✅ Reduces engineering review effort

✅ Improves validation accuracy

✅ Identifies mismatches instantly

✅ Supports telematics fault analysis

✅ Accelerates decision-making process

---

## Technology Stack

- Python
- Pandas
- TQDM

---

## Domain

Automotive Diagnostics  
Vehicle Telematics  
DM1 Fault Analytics  
Engineering Validation Automation

---

## Author

Sanmathi S

Python Developer | Data Analytics | Generative AI | AWS