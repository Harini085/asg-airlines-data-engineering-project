## Power BI Dashboard Demo

A demonstration video of the Power BI dashboard is available here:

[Power BI Dashboard Demo](https://drive.google.com/file/d/1vf4v3xe1LHsZeLI-izg4uADEcfBaVo4n/view?usp=sharing)


# ASG Airlines Data Engineering Project

An end-to-end Data Engineering and Analytics project for the Airlines use case. The project covers raw data ingestion, data profiling, data cleaning, transformation, data validation, analytics-ready dataset generation, Power BI reporting, and project documentation.

## Project Overview

The objective of this project is to transform raw airline data into a clean, structured, validated, and analytics-ready dataset for business analysis and reporting.

The project follows the workflow:

```text
Raw Data
   |
   v
Data Profiling
   |
   v
Data Cleaning
   |
   v
Data Transformation
   |
   v
Data Validation
   |
   v
Analytics-Ready Dataset
   |
   v
Power BI Dashboard
```

The data processing pipeline is implemented using Python and Jupyter Notebook, while Microsoft Power BI is used for visualization and reporting.

## Objectives

* Ingest the raw airline dataset.
* Profile the source data and understand its structure.
* Identify missing values, duplicates, inconsistencies, and data-quality issues.
* Clean and standardize the source data.
* Transform the data into an analytics-ready format.
* Perform data-quality and validation checks.
* Create derived analytical fields.
* Generate the final processed CSV dataset.
* Develop a Power BI dashboard.
* Provide complete technical documentation.
* Maintain the project using Git and GitHub.

## Technology Stack

| Technology         | Purpose                                  |
| ------------------ | ---------------------------------------- |
| Python             | Data processing and transformation       |
| Pandas             | Data cleaning and manipulation           |
| NumPy              | Numerical and data-processing operations |
| Jupyter Notebook   | ETL pipeline development and execution   |
| Microsoft Excel    | Raw source data                          |
| CSV                | Processed analytics-ready dataset        |
| Microsoft Power BI | Dashboard and data visualization         |
| Git                | Version control                          |
| GitHub             | Source-code and project management       |

## Project Architecture

```text
                     Raw Excel Data
                           |
                           v
                  Data Profiling
                           |
                           v
                Data Cleaning & ETL
                           |
                           v
                Data Transformation
                           |
                           v
                  Data Validation
                           |
                           v
             Analytics-Ready CSV Dataset
                           |
                           v
                    Power BI Report
                           |
                           v
                   Business Insights
```

## Project Structure

```text
ASG_Airlines_DataEngineering/
|
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

## Data Source

The raw airline dataset is stored in:

```text
data/raw/Airlines.xlsx
```

The raw dataset is preserved separately from the processed dataset to maintain a clear separation between source data and analytics-ready data.

## Data Profiling

The source dataset is profiled before transformation to understand its structure and identify potential data-quality issues.

The profiling process includes:

* Dataset dimensions
* Column names
* Data types
* Missing-value analysis
* Duplicate-record analysis
* Unique-value analysis
* Cardinality checks
* Numerical statistics
* Categorical analysis
* Date and time validation
* Invalid or inconsistent values
* Potential outlier identification

## Data Engineering Pipeline

The complete ETL pipeline is implemented in:

```text
pipeline/Airlines_Pipeline.ipynb
```

### 1. Extract

The raw Excel dataset is loaded into Python using Pandas.

```text
Airlines.xlsx
     |
     v
Pandas DataFrame
```

### 2. Profile

The dataset is analyzed to identify:

* Missing values
* Duplicate records
* Incorrect data types
* Invalid values
* Inconsistent categorical values
* Data-quality issues

### 3. Clean

The pipeline applies the required data-cleaning operations, including:

* Handling missing values
* Removing or managing duplicates
* Correcting data types
* Standardizing values
* Cleaning inconsistent records
* Processing date and time fields

### 4. Transform

The cleaned dataset is transformed into an analytics-ready structure.

The transformation process includes derived fields such as:

* Flight date
* Route
* Duration in minutes
* Duration in hours
* Overnight flight indicator
* Duration anomaly indicator

### 5. Validate

The transformed dataset is validated to ensure:

* Required columns are available.
* Data types are appropriate.
* Duplicate records are handled.
* Missing values are addressed.
* Invalid values are identified or corrected.
* Derived fields are generated correctly.
* The final dataset is suitable for analytics.

### 6. Load

The final processed dataset is generated at:

```text
data/processed/flights_analytics_ready.csv
```

This dataset is used as the analytical source for Power BI.

## Analytics-Ready Dataset

The processed dataset is available at:

```text
data/processed/flights_analytics_ready.csv
```

The dataset contains analytics-ready fields including:

```text
flight_id
airline
source
destination
route
departure_time
arrival_time
flight_date
duration_minutes
duration_hours
overnight_flag
duration_anomaly_flag
```

The processed dataset provides a clean and structured source for downstream analytics and visualization.

## Data Quality and Validation

The project includes data-quality checks covering:

| Check                   | Purpose                                  |
| ----------------------- | ---------------------------------------- |
| Missing Values          | Identify incomplete records              |
| Duplicate Records       | Prevent duplicate analytical data        |
| Data Types              | Ensure appropriate column types          |
| Categorical Consistency | Standardize categorical values           |
| Date Validation         | Verify date and time fields              |
| Numerical Validation    | Identify invalid numerical values        |
| Output Validation       | Verify the final analytics-ready dataset |

## Power BI Dashboard

The Power BI report is available at:

```text
powerbi/powerbi.pbix
```

The dashboard is designed to provide interactive analysis of the processed airline data.

The analytical areas include:

* Flight analysis
* Airline-level analysis
* Route analysis
* Source and destination analysis
* Flight duration analysis
* Overnight flight analysis
* Duration anomaly analysis
* Time-based analysis
* Interactive filtering and exploration

Open the `.pbix` file using Microsoft Power BI Desktop.

## Power BI Dashboard Demo

A demonstration video of the Power BI dashboard is available here:

[Power BI Dashboard Demo](https://drive.google.com/file/d/1vf4v3xe1LHsZeLI-izg4uADEcfBaVo4n/view?usp=sharing)



## Project Documentation

The detailed project documentation is available at:

```text
documentation/ASG_Airlines_Project_Documentation.docx
```

The documentation covers:

* Project overview
* Requirements
* Architecture
* Data flow
* Data processing approach
* Data transformation
* Data validation
* Data model
* Analytics approach
* Power BI dashboard
* Project implementation

## End-to-End Workflow

```text
                 SOURCE
                   |
                   v
             Airlines.xlsx
                   |
                   v
            DATA PROFILING
                   |
                   v
             DATA CLEANING
                   |
                   v
          DATA TRANSFORMATION
                   |
                   v
           DATA VALIDATION
                   |
                   v
     flights_analytics_ready.csv
                   |
                   v
               POWER BI
                   |
                   v
           BUSINESS INSIGHTS
```

## How to Run the Project

### Prerequisites

Install the following:

* Python 3.x
* Jupyter Notebook or JupyterLab
* Microsoft Power BI Desktop
* Git

### Python Libraries

Install the required Python packages:

```bash
pip install pandas numpy openpyxl jupyter
```

### Step 1: Clone the Repository

Use the actual repository URL:

```bash
git clone https://github.com/Harini085/asg-airlines-data-engineering-project.git
```

Navigate to the repository:

```bash
cd asg-airlines-data-engineering-project
```

Then navigate to the project directory:

```bash
cd ASG_Airlines_DataEngineering
```

### Step 2: Verify the Raw Data

Ensure the source file exists at:

```text
data/raw/Airlines.xlsx
```

### Step 3: Start Jupyter Notebook

Run:

```bash
jupyter notebook
```

Open:

```text
pipeline/Airlines_Pipeline.ipynb
```

### Step 4: Run the ETL Pipeline

Run the notebook cells from top to bottom.

The pipeline reads:

```text
data/raw/Airlines.xlsx
```

and generates:

```text
data/processed/flights_analytics_ready.csv
```

### Step 5: Verify the Output

After successful execution, verify that:

```text
data/processed/flights_analytics_ready.csv
```

has been generated successfully.

### Step 6: Open the Power BI Dashboard

Open:

```text
powerbi/powerbi.pbix
```

using Microsoft Power BI Desktop.

Refresh the dataset if required.

## Data Layers

The project follows a simple layered data architecture.

### Raw Layer

```text
data/raw/
```

Contains the original source dataset.

### Processed Layer

```text
data/processed/
```

Contains the cleaned and transformed analytics-ready dataset.

### Presentation Layer

```text
powerbi/
```

Contains the Power BI report used for visualization and business analysis.

## Data Handling

The project maintains a clear separation between source data, transformation, analytics data, and reporting.

```text
Source Data
     |
     v
Data Transformation
     |
     v
Analytics-Ready Data
     |
     v
Power BI Reporting
```

This approach improves traceability, maintainability, and reproducibility of the data pipeline.

## Key Deliverables

| Deliverable           | Location                                                |
| --------------------- | ------------------------------------------------------- |
| Raw Dataset           | `data/raw/Airlines.xlsx`                                |
| ETL Pipeline          | `pipeline/Airlines_Pipeline.ipynb`                      |
| Processed Dataset     | `data/processed/flights_analytics_ready.csv`            |
| Power BI Dashboard    | `powerbi/powerbi.pbix`                                  |
| Project Documentation | `documentation/ASG_Airlines_Project_Documentation.docx` |
| Dashboard Demo        | Google Drive link provided above                        |

## Project Outcomes

The project demonstrates an end-to-end data engineering workflow by:

* Processing raw airline data.
* Applying data-cleaning and transformation operations.
* Performing data-quality validation.
* Producing a reusable analytics-ready dataset.
* Creating derived analytical fields.
* Connecting processed data to Power BI.
* Providing interactive business analysis.
* Maintaining technical project documentation.
* Providing a reproducible project structure.

## Repository

The complete project is available on GitHub:

https://github.com/Harini085/asg-airlines-data-engineering-project

## Author

**Harini S**

M.Sc. Data Science

## Project Purpose

This project was developed for the ASG Airlines Data Engineering use case and demonstrates practical implementation of data engineering, data quality, analytics-ready data preparation, and business intelligence reporting.
