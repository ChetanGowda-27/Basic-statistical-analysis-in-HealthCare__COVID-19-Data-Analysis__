# Basic Statistical Analysis in Healthcare

## Overview

This project aims to download, preprocess, and perform statistical analysis on ELISA (Enzyme-Linked Immunosorbent Assay) test results, as well as on information related to IgG and IgM antibodies, influenza vaccination, tuberculosis vaccination, previous diseases, and blood group information of the respondents. The goal is to provide insights into healthcare data using statistical techniques and analysis.

## Table of Contents

- [Project Description](#project-description)
- [Data Sources](#data-sources)
- [Data Preprocessing](#data-preprocessing)
- [Statistical Analysis](#statistical-analysis)
- [Project Setup](#project-setup)
  - [Requirements](#requirements)
  - [Installation Instructions](#installation-instructions)
  - [Usage](#usage)
- [File Structure](#file-structure)
- [License](#license)


## Project Description

In this project, we work with datasets related to healthcare information, specifically focusing on:

- **ELISA Tests**: To determine the presence of antibodies (IgG and IgM) which are indicative of immune responses against various pathogens.
- **Vaccination Data**: Information on influenza and tuberculosis vaccinations.
- **Previous Diseases**: Respondent history on diseases they have had.
- **Blood Group Data**: Respondents’ blood group information, which may correlate with vaccine response or disease susceptibility.

The main objective is to explore the relationships and patterns in this data through various statistical techniques. This can assist in drawing meaningful conclusions regarding health trends, vaccination efficacy, and disease prevention strategies.

## Data Sources

The data for this project is collected from different health surveys and ELISA test results. The data points include:

- **IgG and IgM Levels**: Values obtained from ELISA tests.
- **Influenza and Tuberculosis Vaccination History**: Boolean or categorical data indicating whether the individual has been vaccinated.
- **Previous Diseases**: Categorical data indicating the diseases an individual has previously contracted.
- **Blood Group**: Categorical data indicating the respondent's blood group (e.g., A, B, AB, O).

## Data Preprocessing

Before performing any statistical analysis, the data needs to be preprocessed. This involves the following steps:

1. **Data Cleaning**: 
   - Handling missing values.
   - Removing outliers or erroneous data entries.
   - Converting categorical data into numerical format (e.g., encoding vaccination status as 1 for vaccinated and 0 for not vaccinated).

2. **Data Normalization**: 
   - Normalizing the numeric columns (like IgG and IgM levels) to bring them to a similar scale.

3. **Data Transformation**:
   - Encoding textual information such as disease names into categorical numeric values.
   - Combining related features (e.g., grouping individuals by age ranges or by disease history).

4. **Data Visualization**: 
   - Creating initial visualizations to understand distributions and detect any potential data issues (e.g., histograms, bar charts).

## Statistical Analysis

The statistical analysis performed in this project focuses on:

1. **Descriptive Statistics**:
   - Summarizing the basic features of the dataset, including mean, median, variance, and standard deviation for continuous variables such as IgG and IgM levels.
   
2. **Correlation Analysis**:
   - Analyzing the relationship between various factors (e.g., the correlation between vaccination history and antibody levels, or between disease history and IgM presence).

3. **Hypothesis Testing**:
   - Conducting hypothesis tests such as t-tests and chi-square tests to compare groups (e.g., vaccinated vs. non-vaccinated individuals).

4. **Regression Analysis**:
   - Implementing regression models to predict immune response levels (IgG and IgM) based on vaccination status, previous diseases, and blood group.

5. **Statistical Visualization**:
   - Generating plots like scatter plots, box plots, and heatmaps to visualize correlations and trends in the data.

## Project Setup

### Requirements

Before running this project, you need to install the following dependencies:

- Python 3.x
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Statsmodels

You can install these libraries using `pip`:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn statsmodels
```

### Installation Instructions

1. Clone the repository:

```bash
git clone https://github.com/yourusername/Basic-Statistical-Analysis-in-HealthCare.git
```

2. Navigate to the project directory:

```bash
cd Basic-Statistical-Analysis-in-HealthCare
```

3. Install the required dependencies:

```bash
pip install -r requirements.txt
```

### Usage

Once the setup is complete, you can start exploring the data and running the analysis by executing the provided Jupyter notebooks or Python scripts.

To run the project:

For Jupyter Notebook users:

```bash
jupyter notebook
```

Open the notebook `healthcare_analysis.ipynb` and run through the cells.

## File Structure

```
Basic-Statistical-Analysis-in-HealthCare/
├── data/
│   ├── raw_data.csv            # Original dataset
├── notebooks/
│   └── healthcare_analysis.ipynb  # Jupyter notebook for analysis
├── requirements.txt            # List of required libraries
└── README.md                   # Project documentation
```



## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

