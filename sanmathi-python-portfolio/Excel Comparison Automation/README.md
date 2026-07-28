# Excel Data Comparison Automation

## Overview

Excel Data Comparison Automation is a Python-based tool that compares two Excel workbooks (Old Version vs New Version) and automatically identifies differences between them.

The tool performs worksheet-level and cell-level comparison to detect:

- Newly added worksheets
- Newly added data
- Modified data

All detected changes are highlighted in the output Excel file, making document review and change validation faster and more accurate.

---

## How It Works

```text
Old Excel Workbook
        │
        ▼
New Excel Workbook
        │
        ▼
Compare All Sheets
        │
        ▼
Compare Every Cell
        │
        ▼
Detect Differences
        │
        ▼
Generate Highlighted Output Workbook
