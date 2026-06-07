# Data Policy

## Source

Public/sample sales dataset plus original forecasting reference PDF. Larger or private datasets should stay local-only.

`data/raw/real_world_sales_data.csv` is intentionally tracked as sample-safe public input data.

## Folder policy

- `raw/`: local-only raw files or explicitly public sample files.
- `interim/`: local-only working outputs.
- `processed/`: local-only generated datasets.

## Git policy

Raw/private data and generated outputs are ignored by `.gitignore`. Only `.gitkeep` placeholders or explicitly sample-safe files are tracked.

## Claim boundary

This repo demonstrates reproducible forecasting documentation and sample-safe artifact organization. It does not claim a deployed forecasting service or production-grade model monitoring.
