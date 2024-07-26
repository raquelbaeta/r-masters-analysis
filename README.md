# Regression Analysis and Data Processing

## Overview

This repository contains R scripts for performing regression analysis and data processing on a dataset related to seizures and various economic and governance indicators. The analysis includes both logistic regression models and linear regression models, using mixed-effects models where appropriate.

## Installation

To run the scripts, you need to have R installed on your system. Additionally, you need to install the required R packages. You can do this by running the installation commands provided below.

install.packages(c("readr", "tidyverse", "dplyr", "ggplot2", "lme4", "ggeffects", "stargazer", "gridExtra"))

library(readr, tidyverse, dplyr, ggplot2, lme4, ggeffects, stargazer, gridExtra)

## Data

The data used for the analysis is expected to be in RDS format. Ensure the file paths in the script are correct and that the data is available in the specified locations.

## Scripts

### 1. Data Aggregation and Cleaning
The script aggregates data into 3-year intervals and performs necessary cleaning steps. This includes checking for duplicates and handling missing values.

### 2. Logistic Regression Models
Three logistic regression models are created using the glmer function from the lme4 package. The models analyze the relationship between the presence of seizures and various indicators (e.g., UN commitment, governance effectiveness).

model_glmer.GE: Includes Governance Effectiveness.
model_glmer.RL: Includes Rule of Law.
model_glmer.PV: Includes Political Violence.

Predicted probabilities and marginal effects are visualised and saved as PDF files for LaTeX.

### 3. Linear Regression Models
A linear regression model analysing the log of mean seizures across 3-year intervals is also included.

## Results

The results include:

Summary statistics of the models.

Marginal effects and predicted probabilities.

Visualisations of the predicted probabilities.

Combined plots for easy comparison of different models.

All visualisations are saved as PDF and PNG files.


## Contributing

If you have suggestions for improvements or bug fixes, feel free to create an issue or submit a pull request.

## Contact

For any questions or further information, please contact raquel@aside.co.za.
