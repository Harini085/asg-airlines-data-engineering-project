## Power BI Dashboard Demo

 **[Watch the Power BI Dashboard Demonstration](https://drive.google.com/file/d/1vf4v3xe1LHsZeLI-izg4uADEcfBaVo4n/view?usp=sharing)**

The video demonstrates the Power BI dashboard, key visualizations, KPIs, filters, and analytical insights developed from the processed airline dataset.


#  Airlines Data Engineering Project

An end-to-end **Data Engineering and Analytics project** built for the Airlines use case. The project covers raw data ingestion, data profiling, data cleaning and transformation, generation of an analytics-ready dataset, and business intelligence visualization using Power BI.

---

##  Project Overview

The objective of this project is to transform raw airline data into a clean, structured, and analytics-ready dataset that can be used to derive meaningful business insights.

The project follows a simple end-to-end data engineering workflow:

**Raw Data → Data Profiling → Data Cleaning & Transformation → Processed Dataset → Power BI Dashboard**

The solution is implemented using Python and Jupyter Notebook for data processing and Power BI for analytics and visualization.

---

##  Objectives

* Understand and profile the raw airline dataset.
* Identify missing values, duplicates, inconsistencies, and data-quality issues.
* Clean and transform the source data.
* Standardize data types and values.
* Generate an analytics-ready dataset.
* Perform data-quality validation.
* Build a Power BI dashboard for business analysis.
* Maintain project documentation covering the architecture, data flow, and data model.

---

##  Project Architecture

```text
                    ┌──────────────────────┐
                    │     Raw Excel Data   │
                    │      Airlines.xlsx   │
                    └──────────┬───────────┘
                               │
                               ▼
                    ┌──────────────────────┐
                    │   Data Profiling     │
                    │  Quality Assessment  │
                    └──────────┬───────────┘
                               │
                               ▼
                    ┌──────────────────────┐
                    │ Data Cleaning & ETL  │
                    │   Python / Pandas    │
                    └──────────┬───────────┘
                               │
                               ▼
                    ┌──────────────────────┐
                    │ Processed Dataset    │
                    │ Analytics-Ready CSV  │
                    └──────────┬───────────┘
                               │
                               ▼
                    ┌──────────────────────┐
                    │      Power BI        │
                    │ Dashboard & Insights │
                    └──────────────────────┘
```

---

##  Technology Stack

| Technology           | Purpose                                      |
| -------------------- | -------------------------------------------- |
| **Python**           | Data processing and transformation           |
| **Pandas**           | Data cleaning and manipulation               |
| **Jupyter Notebook** | ETL pipeline development and execution       |
| **Excel**            | Raw source data                              |
| **CSV**              | Processed analytics-ready dataset            |
| **Power BI**         | Data visualization and dashboard development |
| **Git & GitHub**     | Version control and project management       |

---

##  Project Structure

```text
ASG_Airlines_DataEngineering/
│
├── data/
│   ├── raw/
│   │   └── Airlines.xlsx
│   │
│   └── processed/
│       └── flights_analytics_ready.csv
│
├── pipeline/
│   └── Airlines_Pipeline.ipynb
│
├── powerbi/
│   └── powerbi.pbix
│
├── documentation/
│   └── ASG_Airlines_Project_Documentation.docx
│
└── README.md
```

---

##  Data Source

The raw airline data is provided in Excel format.

```text
data/raw/Airlines.xlsx
```

The raw dataset is treated as the source layer and is not directly used for dashboard reporting.

---

##  Data Profiling

Before transformation, the source data is profiled to understand its structure and data quality.

The profiling process includes:

* Dataset dimensions
* Column names and data types
* Missing-value analysis
* Duplicate-record analysis
* Unique-value analysis
* Cardinality checks
* Invalid or inconsistent values
* Numerical-column statistics
* Categorical-column analysis
* Date-column validation
* Potential outlier identification
* Data-quality observations

The profiling stage helps identify issues before the transformation pipeline is executed.

---

## ⚙️ Data Engineering Pipeline

The ETL pipeline is implemented in:

```text
pipeline/Airlines_Pipeline.ipynb
```

### Pipeline Flow

### 1. Extract

The raw Excel file is loaded into Python using Pandas.

```text
Airlines.xlsx
       ↓
    Pandas
```

### 2. Profile

The dataset is analyzed to identify:

* Missing values
* Duplicate records
* Incorrect data types
* Invalid values
* Inconsistent categorical values
* Data-quality issues

### 3. Transform

The pipeline performs the required data transformations, including:

* Handling missing values
* Removing duplicate records
* Correcting data types
* Standardizing categorical values
* Cleaning inconsistent records
* Formatting date-related fields
* Validating transformed data

### 4. Validate

The transformed dataset is checked to ensure:

* Required columns are available.
* Data types are appropriate.
* Duplicate records are handled.
* Missing values are addressed according to the transformation rules.
* Invalid values are identified or corrected.
* The final dataset is suitable for analytics.

### 5. Load

The final analytics-ready dataset is written to:

```text
data/processed/flights_analytics_ready.csv
```

This processed dataset is then used as the analytical source for Power BI.

---

##  Analytics-Ready Dataset

The processed output is available at:

```text
data/processed/flights_analytics_ready.csv
```

The purpose of this layer is to provide a clean and consistent dataset for downstream analytics and reporting.

Instead of connecting Power BI directly to the raw source, the dashboard uses the transformed analytics-ready data.

---

## 📈 Power BI Dashboard

The Power BI report is available at:

```text
powerbi/powerbi.pbix
```

The dashboard provides an analytical view of the airline data and enables users to explore relevant business metrics and trends.

Typical analytical areas include:

* Flight performance
* Airline-level analysis
* Route analysis
* Passenger-related metrics
* Revenue or financial metrics where available
* Operational trends
* Time-based analysis
* Comparative business performance

> Open the `.pbix` file using Microsoft Power BI Desktop.

---

## 📚 Project Documentation

Detailed project documentation is available in:

```text
documentation/ASG_Airlines_Project_Documentation.docx
```

The documentation contains the project's technical and functional details, including:

* Project overview
* Requirements
* Architecture
* Data flow
* Data processing approach
* Data model
* Transformation logic
* Analytics approach
* Dashboard information

---

##  End-to-End Workflow

```text
                    SOURCE
                      │
                      ▼
             Airlines.xlsx
                      │
                      ▼
               DATA PROFILING
                      │
                      ▼
             DATA CLEANING
                      │
                      ▼
            DATA TRANSFORMATION
                      │
                      ▼
             DATA VALIDATION
                      │
                      ▼
        flights_analytics_ready.csv
                      │
                      ▼
                POWER BI
                      │
                      ▼
             BUSINESS INSIGHTS
```

---

##  How to Run the Project

### Prerequisites

Install the following:

* Python 3.x
* Jupyter Notebook / JupyterLab
* Microsoft Power BI Desktop

### Python Libraries

Install the required Python packages:

```bash
pip install pandas openpyxl jupyter
```

---

### Step 1 — Clone the Repository

```bash
git clone <YOUR_GITHUB_REPOSITORY_URL>
```

Navigate into the project directory:

```bash
cd ASG_Airlines_DataEngineering
```

---

### Step 2 — Verify the Raw Data

Ensure the source file is available at:

```text
data/raw/Airlines.xlsx
```

---

### Step 3 — Run the ETL Pipeline

Launch Jupyter Notebook:

```bash
jupyter notebook
```

Open:

```text
pipeline/Airlines_Pipeline.ipynb
```

Run the notebook cells from top to bottom.

---

### Step 4 — Verify the Output

After successful execution, verify that the processed dataset is available at:

```text
data/processed/flights_analytics_ready.csv
```

---

### Step 5 — Open the Power BI Dashboard

Open:

```text
powerbi/powerbi.pbix
```

in **Microsoft Power BI Desktop**.

Refresh the dataset if required.

---

##  Data Quality Checks

The pipeline performs data-quality checks to improve the reliability of the analytical dataset.

| Check                   | Purpose                              |
| ----------------------- | ------------------------------------ |
| Missing Values          | Identify incomplete records          |
| Duplicate Records       | Prevent duplicate analytical data    |
| Data Types              | Ensure columns use appropriate types |
| Categorical Consistency | Standardize values                   |
| Date Validation         | Ensure valid date representations    |
| Numerical Validation    | Identify invalid numerical values    |
| Output Validation       | Verify the final dataset             |

---

##  Data Layers

The project follows a simple layered data approach:

### Raw Layer

```text
data/raw/
```

Contains the original source data without transformation.

### Processed Layer

```text
data/processed/
```

Contains cleaned and transformed data prepared for analytics.

### Presentation Layer

```text
powerbi/
```

Contains the Power BI report used for visualization and business analysis.

---

##  Data Handling

The raw source data is preserved separately from the processed output.

This provides a clear separation between:

```text
Source Data
     ↓
Transformation
     ↓
Analytics Data
     ↓
Reporting
```

This approach makes the pipeline easier to understand, validate, and maintain.

---

##  Key Deliverables

| Deliverable           | Location                                                |
| --------------------- | ------------------------------------------------------- |
| Raw Dataset           | `data/raw/Airlines.xlsx`                                |
| ETL Pipeline          | `pipeline/Airlines_Pipeline.ipynb`                      |
| Processed Dataset     | `data/processed/flights_analytics_ready.csv`            |
| Power BI Dashboard    | `powerbi/powerbi.pbix`                                  |
| Project Documentation | `documentation/ASG_Airlines_Project_Documentation.docx` |

---

##  Key Outcomes

The project demonstrates an end-to-end data engineering workflow by:

* Converting raw airline data into structured analytical data.
* Applying data-quality and transformation processes.
* Producing a reusable analytics-ready dataset.
* Connecting processed data to a BI reporting layer.
* Providing a documented and reproducible data pipeline.

---

## Author

**Harini S**
M.sc Data Science
