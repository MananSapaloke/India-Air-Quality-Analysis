# India Air Quality Analysis & Visualization Dashboard

### A comprehensive, end-to-end data analytics project showcasing ETL, data modeling, and interactive business intelligence.

---

### 🔴 [Live Interactive Dashboard Link]([YOUR-POWER-BI-PUBLISH-TO-WEB-LINK-HERE])

---

## Table of Contents
- [Project Objective](#project-objective)
- [Technology Stack](#technology-stack)
- [Data Architecture](#data-architecture)
- [Key Features & Analysis](#key-features--analysis)
- [Dashboard Showcase](#dashboard-showcase)
- [Author](#author)


## Project Objective

The goal of this project is to provide a powerful and intuitive tool for analyzing air quality data across India. By transforming raw, complex datasets into a clean, interactive dashboard, this project aims to uncover meaningful patterns and insights into pollution trends. It demonstrates a complete data analytics workflow, from initial data processing and storage to advanced modeling and final visualization, making complex data accessible to both technical and non-technical audiences.

## Technology Stack

A combination of robust data processing tools and business intelligence software was used to build this project from the ground up.

| Technology | Purpose |
| :--- | :--- |
| **Python** | For the core ETL process, including data cleaning, transformation, and validation using the **Pandas** library. |
| **SQL** | For data storage and management within a centralized **SQLite** database, establishing a single source of truth. |
| **Power BI** | For the entire business intelligence layer, including: <br> • **Power Query (M Language):** Initial data shaping. <br> • **Data Modeling:** Building a robust Star Schema. <br> • **DAX:** Authoring advanced measures for dynamic calculations. <br> • **Visualization:** Designing all charts, maps, and interactive elements. |
| **Git / GitHub** | For version control and project documentation. |

## Data Architecture

The project follows a structured, multi-stage data pipeline to ensure data integrity and report performance.



1.  **Extraction:** Raw data is ingested from multiple large CSV files.
2.  **Transformation:** A Python script using Pandas cleans the data, handles missing values, standardizes formats, and creates new features (e.g., 'Agency').
3.  **Loading:** The cleaned data is loaded into a structured SQLite database, separating dimensions (like Stations) from facts (like daily and hourly readings).
4.  **Modeling & Visualization:** Power BI connects to the SQLite database, where a Star Schema model is built to relate the tables. All visuals and DAX measures are then built on top of this efficient model.

## Key Features & Analysis

This dashboard is more than just a collection of charts; it's an analytical tool packed with features:

- **Dynamic Pollutant Analysis:** Users can select any of the 8 major pollutants (PM2.5, SO2, etc.) to dynamically pivot all visuals on the "Pollutant Specific Analysis" page.
- **Time-Series Intelligence:** The report includes Year-over-Year (YoY) comparisons to track long-term trends and identify whether air quality is improving or worsening.
- **Hourly & Seasonal Pattern Recognition:** Dedicated pages allow for the deep-dive analysis of 24-hour pollution cycles (identifying rush-hour peaks) and month-wise seasonal trends.
- **Interactive Filtering:** All visuals are interconnected. Slicing by State, City, or Year allows for a seamless drill-down from a national overview to a hyper-local view.
- **Data-Driven Insights:** The dashboard successfully uncovers key insights, such as the strong correlation between traffic-related pollutants (NO2, CO) and the severe winter pollution spikes in northern states.

## Dashboard Showcase

#### 1. Executive Summary / Overview
*A high-level view of the key performance indicators (KPIs) and geographical distribution of air quality.*
![Overview Page](./1\)%20Overview.jpg)

#### 2. Pollutant Specific Analysis
*An interactive deep-dive tool to analyze the behavior and impact of individual chemical pollutants.*
![Pollutant Analysis Page](./3\)%20Pollutant%20Specific%20Analysis.jpg)

#### 3. Monthwise & Hourly Analysis
*Granular views for identifying seasonal and daily pollution patterns.*
![Monthwise Page](./4\)%20Monthwise%20Analysis.jpg)
![Hourly Page](./5\)%20Hourly%20Analysis.jpg)

#### 4. Documentation
*An 'About' page containing project metadata, data source information, and user guidance.*
![Documentation Page](./6\)%20Documentation.jpg)


## Author

**Manan Sapaloke**

- **LinkedIn:** [https://www.linkedin.com/in/manansapaloke](https://www.linkedin.com/in/manansapaloke)
- **GitHub:** [https://github.com/MananSapaloke](https://github.com/MananSapaloke)
