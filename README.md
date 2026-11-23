# Earthquake Data Engineering & Analytics – Microsoft Fabric and Power BI

## Project Overview

This project implements an end-to-end Data Engineering and Business Intelligence solution for analyzing worldwide earthquake events using data from the [USGS Earthquake API](https://earthquake.usgs.gov/fdsnws/event/1/).

The solution uses **Microsoft Fabric** to ingest, process, and organize earthquake data following the Medallion Architecture (Bronze, Silver, and Gold layers), with **Power BI** as the data visualization and analytics platform.

## Architecture

The project is designed around the following workflow:

1. **Data Source:** Retrieve earthquake event data from the USGS API.
2. **Data Ingestion:** Use Microsoft Fabric Data Factory to orchestrate the ingestion process.
3. **Data Processing:** Use Fabric Notebooks and Python to extract, transform, and prepare the data.
4. **Data Storage:** Store the data in a Microsoft Fabric Lakehouse.
5. **Data Analytics:** Build analytical datasets and reports using Power BI.

## Medallion Architecture

The data pipeline follows the Medallion Architecture:

| Layer | Description |
|---|---|
| Bronze | Raw earthquake data extracted from the USGS API and stored in its original JSON format. |
| Silver | Cleaned, validated, and transformed earthquake records. |
| Gold | Curated datasets structured for analytical queries and Power BI reporting. |

## Technologies

- **Microsoft Fabric**
- **Microsoft Fabric Data Factory**
- **Microsoft Fabric Lakehouse**
- **Python**
- **PySpark**
- **REST APIs**
- **Power BI**
- **GitHub**

## Data Source

The project uses the official USGS Earthquake API:

https://earthquake.usgs.gov/fdsnws/event/1/

The API provides earthquake information such as:

- Magnitude
- Location
- Geographic coordinates
- Depth
- Event timestamp
- Place description

## Repository Structure

```text
earthquake-data-engineering-microsoft-fabric-power-bi/
│
├── notebooks/
│   └── 01_Worldwide_Earthquake_Events_API_Bronze_Layer.ipynb
│
├── README.md
└── ...
```

## Project Objectives

- Develop an end-to-end data ingestion and processing pipeline.
- Work with external REST APIs.
- Implement the Medallion Architecture using Microsoft Fabric.
- Apply data engineering concepts using Python and PySpark.
- Prepare structured datasets for Business Intelligence.
- Create interactive Power BI dashboards to explore worldwide earthquake activity.

## Status

This repository documents the development of the project. Additional components, including the Silver and Gold layers, orchestration, and Power BI reporting, will be added as the solution evolves.
