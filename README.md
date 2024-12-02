# DATA-512-PART-4

This repository contains all the components necessary for the course project, showcasing a comprehensive, impactful, and reproducible analysis as part of a human-centered data science framework.

## Repository Structure

### 1. Written Report

The `report/` directory contains a detailed report with the following sections:

- **Introduction:** Context and significance of the research question.
- **Background/Related Work:** Summary of prior studies and their impact on this analysis.
- **Methodology:** Analytical techniques and ethical considerations.
- **Findings:** Results with clear visualizations and narrative explanations.
- **Discussion/Implications:** Actionable insights for stakeholders.
- **Limitations:** Data, methodological, and statistical constraints.
- **Conclusion:** Key takeaways and broader implications.
- **References/Data Sources:** Comprehensive citations and data descriptions.

### 2. Code Documentation

The `notebooks/` directory includes Jupyter notebooks with:

- Fully documented steps for analysis.
- Markdown cells explaining each step and its purpose.
- Clear outputs demonstrating key results.

### 3. Data Documentation

The `data/` directory contains:

- Raw data files used in the analysis.
- Intermediate files generated during preprocessing.
- A `README.md` file describing each data file and its source.
- Links to external datasets (e.g., EPA AQI API, Ephtracking government datasets).

### 4. Supporting Materials

The `extras/` directory contains:

- Supplementary scripts, models, and other materials.
- A `README.md` file describing their purpose.

### 5. README File

This `README.md` provides:

- An overview of the repository structure.
- Instructions for reproducing results.
- Dependencies and setup instructions.

### 6. LICENSE File

The repository includes a `LICENSE` file specifying usage permissions (e.g., MIT or GPL).

## Instructions for Reproducing Results

1. Clone this repository:
   ```bash
   git clone <repository_link>
   cd <repository_name>
   ```
2. Set up the required environment:
   - Install Python dependencies listed in `requirements.txt`:
     ```bash
     pip install -r requirements.txt
     ```
   - Ensure access to the necessary datasets.
3. Navigate to the `notebooks/` directory and execute the Jupyter notebooks in sequence.
4. Refer to the `report/` directory for detailed interpretations of the results.

## Dependencies

- Python 3.8+
- Jupyter Notebook
- pandas, numpy, matplotlib, scipy, scikit-learn

## Project Objectives

This project aims to analyze and interpret air quality and health data for the assigned US city, focusing on human-centered considerations. By integrating diverse datasets and leveraging analytical models, the project identifies trends, evaluates policy impacts, and provides actionable insights for stakeholders.

---

### Project Overview

This project explores biases in air quality and health data by analyzing asthma hospitalizations and air pollution metrics in a U.S. city. The objective is to understand how environmental and policy factors influence health outcomes, reflecting principles of human-centered data science.

**Goals:**

- **Trend Analysis:** Evaluate air quality trends and their relationship to asthma hospitalizations.
- **Impact of Policies:** Assess how health-focused policies introduced after 2016 affected hospitalization rates.
- **Human-Centered Insights:** Provide actionable recommendations for stakeholders.

### Research Implications

- **Health Impacts of Pollution:** Analysis demonstrates correlations between poor air quality and increased asthma hospitalizations.
- **Policy Effectiveness:** Results indicate a significant decrease in hospitalizations post-policy changes, suggesting effective interventions.
- **Bias and Data Limitations:** Highlights potential biases in data collection (e.g., geographic or temporal biases) and their implications for public health research.

### APIs and Data Sources

#### Data Sources

- **EPA AQI API:** Provides air quality data such as mean PM2.5 levels, smoke days, and severe smoke days. Available at: [EPA Air Quality System (AQS) Data API](https://aqs.epa.gov/aqsweb/documents/data_api.html).
- **Ephtracking Government Dataset:** Offers asthma hospitalization data at the county level from 1999 to 2021. Accessed from: [Ephtracking Data Portal](https://ephtracking.cdc.gov/).

#### APIs Used

- **EPA AQS API:** Used to fetch AQI and PM2.5-related data. API documentation available at the EPA AQS website.
- **Data Retrieval:** Data was programmatically retrieved using Python scripts to interact with the API endpoints, ensuring accurate and up-to-date information.

#### Accessing APIs and Downloading Data

- **EPA AQS API:**

  - To access this API, register for an account at the EPA AQS portal and obtain an API key.
  - Query examples include retrieving PM2.5 or AQI data for specific locations and timeframes.
  - Data structure includes fields like `Date`, `PM2.5 Levels`, `AQI`, `Smoke Impact Days`, and `Severe Smoke Days`.

- **Ephtracking Dataset:**

  - Data can be downloaded directly from the Ephtracking portal in CSV format. Filters for county-level asthma hospitalization data can be applied before downloading.
  - Data structure includes fields like `Year`, `County`, `Hospitalization Rates`, and `Total Hospitalizations`.

#### Data Provenance

- **Asthma Data:** Cleaned and processed from the Ephtracking dataset to include only relevant fields for the analysis.
- **Air Quality Data:** Fetched and preprocessed from EPA AQS API to align with the temporal and geographic scope of the study.

#### CSVs Used in the Analysis

- **`Hampden_Asthma.csv`****:** Contains county-level data on asthma hospitalization rates and total hospitalizations from 1999 to 2021.
- **`Springfield_AQI.csv`****:** Includes year-wise air quality metrics such as PM2.5 levels and smoke impact scores for Springfield.
- **Merged Dataset:** Combines asthma hospitalization and AQI data for comprehensive analysis. Generated as part of the preprocessing step.

---

For more details, refer to the written report in the `report/` directory or contact the repository maintainer.

