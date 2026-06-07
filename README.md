# Sales Forecasting Decision Support

How can a sales dataset become a reproducible forecasting decision-support artifact with clear public limitations?

## Business question

How can a sales dataset become a reproducible forecasting decision-support artifact with clear public limitations?

## Reviewer guide

1. `data/raw/real_world_sales_data.csv` — sample-safe public input data.
2. `references/Application-of-PyCaret-AutoML-for-Sales-Forecasting.pdf` — original forecasting reference artifact.
3. `docs/evaluation.md` and `reports/results.md` — verification notes.
4. `scripts/verify.py` — smoke verifier.

## Data source

Public/sample sales dataset plus original forecasting reference PDF. Larger or private datasets should stay local-only.

## Repository structure

```text
README.md
LICENSE
.gitignore
requirements.txt
data/
  raw/          # source/sample input files or local-only raw data
  interim/      # local-only transformed working files
  processed/    # local-only generated datasets
notebooks/      # ordered analysis notebooks/scripts
src/            # reusable project code
dashboard/      # BI/dashboard files or dashboard export code
docs/           # documentation and evaluation notes
reports/        # human-readable findings and figures
references/     # source notes, papers, dictionaries, original materials
scripts/        # verification or utility scripts
```

## Setup

```bash
python -m venv .venv
source .venv/bin/activate
python -m pip install --upgrade pip
python -m pip install -r requirements.txt
```

## Run / verify

```bash
python3 scripts/verify.py
```

## Public outputs

- Dashboard or public artifact: `Sample data, forecasting reference document, and verification evidence.`
- Findings and evidence notes: `reports/`
- Evaluation notes: `docs/`
- Supporting references: `references/`

## Claim boundary

This repo demonstrates reproducible forecasting documentation and sample-safe artifact organization. It does not claim a deployed forecasting service or production-grade model monitoring.

## Data and security policy

- Credentials, environment files, local raw data, generated working data, databases, archives, and scratch outputs are ignored by `.gitignore`.
- Public repo keeps only shareable code, sample-safe artifacts, documentation, dashboard files, and evidence summaries.
- Claims stay bounded by available data and documented assumptions.
