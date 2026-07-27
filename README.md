# Cervical Cancer Risk Factors: Exploratory Data Analysis

## Overview

In this project, an exploratory data analysis (EDA) is performed on the Cervical Cancer Risk Factors dataset obtained from the UCI Machine Learning Repository. The purpose of this EDA is to examine, clean, and analyze the dataset in order to explore relationships between the dataset's features (risk factors) and cervical cancer diagnostic outcomes.

## Dataset

The dataset contains features regarding demographics, lifestyle, medical history, and test results from a total of 858 patients. It was collected at 'Hospital Universitario de Caracas' in Caracas, Venezuela. 

The diagnostic outcome variables are:

- Hinselmann
- Schiller
- Citology
- Biopsy

Dataset source: 

Fernandes, K., Cardoso, J., & Fernandes, J. (2017). Cervical Cancer (Risk Factors) [Dataset]. UCI Machine Learning Repository. https://doi.org/10.24432/C5Z310.

## Objectives

The goal of this project is to explore the Cervical Cancer Risk Factors dataset by cleaning the dataset, analyzing feature distribution, identifying correlation between variables, and finally examining associations with screening outcomes.

## Data Cleaning

Cleaning missing values includes either removing columns entirely or imputing them with the median for quantitative variables and the mode for categorical variables.

Since the two variables, STDs: Time since first diagnosis and STDs: Time since last diagnosis have around 92% of their data missing (787/857), they should be dropped since they have insufficient data for meaningful analysis.

After completing this step, the dataset contained 858 complete observations across all remaining features.

## Exploratory Analysis

The following methods to conduct this EDA were used:

- Dataset inspection
- Descriptive statistics
- Heat map visualization
- Count plot visualization of target variables
- Box plot comparisons between biopsy outcomes and certain variables

## Key Findings

- In general, positive test outcomes are relatively rare compared to negative outcomes, which results in large class imbalances.
- Many individual variables exhibited a weak correlation with biopsy outcomes.
- The box plots demonstrated large amounts of overlap between both positive and negative biopsy groups, which suggests that no individual feature is sufficient to separate the classes.
- Many risk factor variables had very uneven distribution, such as heavily right skewed features and features where a majority of the participants answered 'no' to certain risk factors.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook
