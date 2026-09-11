# Airlines Use Case Project

## Overview
This project contains the end-to-end data pipeline, analysis, and dashboard
for the Airlines use case.

## Folder Structure
- `data/raw/` — Original source data (UseCase - Airlines.xlsx)
- `data/processed/` — Cleaned CSV outputs (flights, bookings, passengers, payments)
- `pipeline/` — Jupyter notebook containing the data pipeline/ETL logic
- `powerbi/` — Power BI dashboard (.pbix)
- `documentation/` — Architecture, data flow, data model diagrams, and project documentation
- `logs/` — Pipeline execution/validation logs

## How to Use
1. Place the raw source file in `data/raw/`.
2. Run the notebook in `pipeline/airlines_pipeline.ipynb` to generate cleaned CSVs in `data/processed/`.
3. Open `powerbi/Airlines_Dashboard.pbix` to view the dashboard, refreshing the data source as needed.
4. Refer to `documentation/` for architecture and data model details.
5. Check `logs/pipeline_validation.log` for pipeline run/validation history.
