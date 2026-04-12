# NYC TLC Azure Data Platform

An end-to-end Azure data engineering platform built on NYC Taxi & Limousine Commission (TLC) 2025 trip data.

## Architecture

| Project | Description | Services |
|---|---|---|
| P1 | Data Ingestion | ADF, ADLS Gen2, Key Vault |
| P2 | Medallion Architecture | Databricks, Delta Lake |
| P3 | Data Warehouse & Reporting | Synapse Analytics, Power BI |
| P4 | Real-time Streaming | Event Hubs, Stream Analytics |
| P5 | Data Quality & Observability | Great Expectations, Azure Monitor |

## Dataset

Source: [NYC TLC Trip Record Data](https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page)
- Yellow Taxi, Green Taxi, FHV, HVFHV trip records
- Year: 2025 (all 12 months)
- Format: Parquet
- Total files: 48

## Tech Stack

- **Ingestion** — Azure Data Factory
- **Storage** — Azure Data Lake Storage Gen2
- **Transformation** — Azure Databricks, Delta Lake
- **Warehousing** — Azure Synapse Analytics
- **Visualization** — Power BI
- **Streaming** — Azure Event Hubs, Stream Analytics
- **Quality** — Great Expectations, Azure Monitor
- **Security** — Azure Key Vault, RBAC

## Project Structure

```
nyc-tlc-azure-data-platform/
├── adf/                  # Azure Data Factory pipelines, datasets, linked services
├── notebooks/            # Databricks transformation notebooks (Project 2)
├── synapse/              # Synapse SQL scripts and schemas (Project 3)
├── streaming/            # Stream Analytics queries (Project 4)
├── quality/              # Great Expectations configs and checkpoints (Project 5)
└── docs/                 # Architecture diagrams and documentation
```
## Setup Instructions

### Prerequisites
- Azure subscription
- GitHub account
- Azure CLI installed

### Resources Required
- Resource Group: `rg-nyc-tlc-dev-eastus`
- ADLS Gen2: `dlsnycldeveastus`
- Key Vault: `kv-nyc-tlc-dev-eastus`
- Data Factory: `adf-nyc-tlc-dev-eastus`

## Status

- [x] P1 — Data Ingestion (In Progress)
- [ ] P2 — Medallion Architecture
- [ ] P3 — Data Warehouse & Reporting
- [ ] P4 — Real-time Streaming
- [ ] P5 — Data Quality & Observability
