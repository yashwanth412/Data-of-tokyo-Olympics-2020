# Tokyo Olympics 2020 — End-to-End Data Engineering Pipeline

> A complete cloud-native data engineering project built on Microsoft Azure, demonstrating ETL pipeline development, data transformation, and business intelligence dashboarding.

[![Azure](https://img.shields.io/badge/Azure-Cloud-blue)](https://azure.microsoft.com/)
[![Python](https://img.shields.io/badge/Python-3.8+-yellow)](https://www.python.org/)
[![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-yellowgreen)](https://powerbi.microsoft.com/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

---

## Project Overview

This project implements a production-grade **ETL data pipeline** for the Tokyo Olympics 2020 dataset, leveraging **Microsoft Azure** services to ingest, transform, model, and visualize Olympic Games data.

### Business Problem
Sports organizations and analysts need centralized, clean, and actionable data to derive insights on athlete performance, medal distributions, country-wise statistics, and event trends. This pipeline automates the entire data lifecycle from raw ingestion to executive-ready dashboards.

### Solution Architecture
```
Raw Data (CSV/JSON)
    ↓
Azure Storage (Data Lake Gen2)
    ↓
Azure Data Factory (Orchestration & Ingestion)
    ↓
Azure Synapse Analytics (Data Warehousing)
    ↓
Azure Databricks (Transformation & Modeling — Python/SQL)
    ↓
Power BI (Visualization & Reporting)
    ↓
Azure Synapse Workspace (Published Dashboards)
```

---

## Tech Stack

| Layer | Technology |
|-------|------------|
| **Cloud Platform** | Microsoft Azure |
| **Orchestration** | Azure Data Factory |
| **Data Warehouse** | Azure Synapse Analytics |
| **Transformation** | Azure Databricks (PySpark, SQL) |
| **Storage** | Azure Data Lake Storage Gen2 |
| **Visualization** | Microsoft Power BI |
| **Languages** | Python, SQL, PySpark |
| **Version Control** | Git |

---

## Key Features

- **End-to-End ETL Pipeline**: Automated data ingestion, transformation, and loading using Azure Data Factory pipelines
- **Data Modeling**: Star schema design in Synapse for optimized analytical queries
- **Data Quality**: Validation checks, null handling, and deduplication at each pipeline stage
- **Scalable Processing**: Databricks clusters for distributed data transformation on large datasets
- **Interactive Dashboards**: Power BI reports with drill-down capabilities for country, sport, and athlete-level insights
- **Cloud-Native**: Fully serverless architecture with Azure-managed services

---

## Dataset

The dataset includes:
- **Athletes**: 11,000+ athlete profiles with country, sport, and event details
- **Coaches**: Coaching staff information by country and discipline
- **EntriesGender**: Gender-wise participation counts per sport
- **Medals**: Medal tallies by country (Gold, Silver, Bronze)
- **Teams**: Team-based event registrations

---

## Project Structure

```
Data-of-tokyo-Olympics-2020/
├── data/
│   ├── raw/                    # Raw source files
│   └── processed/              # Cleaned & transformed data
├── notebooks/
│   ├── 01_data_ingestion.ipynb
│   ├── 02_data_cleaning.ipynb
│   ├── 03_data_transformation.ipynb
│   └── 04_data_modeling.ipynb
├── pipelines/
│   ├── adf_pipeline.json       # Azure Data Factory pipeline definition
│   └── synapse_queries.sql     # SQL scripts for Synapse
├── powerbi/
│   └── tokyo_olympics_dashboard.pbix
├── docs/
│   └── architecture_diagram.png
└── README.md
```

---

## Skills Demonstrated

- **Data Engineering**: ETL/ELT pipeline design, data orchestration, data warehousing
- **Cloud Computing**: Azure Synapse, Azure Data Factory, Azure Databricks, Azure Storage
- **Data Transformation**: PySpark, SQL, data cleaning, data modeling
- **Business Intelligence**: Power BI dashboard development, DAX measures, data storytelling
- **Data Quality**: Schema validation, data profiling, error handling
- **Project Management**: End-to-end project delivery from raw data to stakeholder-ready insights

---

## Dashboard Preview

*(Add screenshots of your Power BI dashboard here)*

> Example insights delivered:
> - Top 10 medal-winning countries
> - Gender distribution across sports
> - Athlete participation by continent
> - Medal trend analysis by sport category

---

## How to Run

> **Note**: This project requires an active Azure subscription.

1. **Clone the repository**
   ```bash
   git clone https://github.com/yashwanth412/Data-of-tokyo-Olympics-2020.git
   cd Data-of-tokyo-Olympics-2020
   ```

2. **Set up Azure resources**
   - Create an Azure Storage Account (Data Lake Gen2)
   - Deploy Azure Synapse Analytics workspace
   - Create an Azure Data Factory instance
   - Provision an Azure Databricks workspace

3. **Run the pipeline**
   - Upload raw data to Azure Storage
   - Execute ADF pipeline for data ingestion
   - Run Databricks notebooks for transformation
   - Load processed data into Synapse SQL pool
   - Connect Power BI to Synapse for visualization

---

## Future Enhancements

- [ ] Implement incremental data loading (delta processing)
- [ ] Add CI/CD pipeline using Azure DevOps
- [ ] Integrate real-time streaming with Azure Event Hubs
- [ ] Deploy ML models for medal prediction
- [ ] Add data lineage tracking with Azure Purview

---

## Connect With Me

- **Email**: pasupuleti.yashwanth0412@gmail.com
- **Portfolio**: [github.com/yashwanth412](https://github.com/yashwanth412)

---

## License

This project is licensed under the MIT License.

About Dataset
Details
This contains the details of over 11,000 athletes, with 47 disciplines, along with 743 Teams taking part in the 2021(2020) Tokyo Olympics.
This dataset contains the details of the Athletes, Coaches, Teams participating as well as the Entries by gender. It contains their names, countries represented, discipline, gender of competitors, name of the coaches.

Will update the dataset with medals(gold, silver, bronze), more details about the athletes after few weeks.

Credits
Source: Tokyo Olympics 2020 Website

