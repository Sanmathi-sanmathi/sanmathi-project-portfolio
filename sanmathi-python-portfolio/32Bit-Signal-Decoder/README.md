# 32Bit Signal Decoder

## What This Project Does

This tool converts a decimal value into a 32-bit binary format and decodes signal information from the generated bit values.

## Input

```text
Decimal Value

Example:
20501
```

## Processing

- Convert decimal to 32-bit binary
- Split binary into 16 groups of 2 bits
- Convert each group into decimal values
- Map values to diagnostic signals

## Output

```text
32-bit Binary Value

2-bit Chunks

Signal Status Values
```

### Example Signals

- AC Request Switch
- Pressure Switch Status
- Thermo Amplifier Status
- Compressor Relay Status
- Engine RPM Increase Relay Status

## Tech Stack

- Python

## Business Value

✅ Decodes binary signal data automatically

✅ Eliminates manual bit calculations

✅ Simplifies diagnostics analysis

✅ Improves troubleshooting efficiency

## Domain

Automotive Diagnostics | Embedded Systems

## Author

Sanmathi S