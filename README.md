# Project-4-Team-3
Project 4 Air Quality assessment 
# Objective:
**AIR QUALITY**
Air pollution is a critical environmental threat impacting urban populations, particularly in New York City (NYC). This project aims to analyze NYC air quality data to understand pollutant levels, their distribution across neighborhoods, temporal trends, and spatial patterns. The analysis will focus on pollutants such as PM 2.5 and SO2, providing insights into their impacts on public health.
# Analysis Questions:
- What are the average, median, and variability of PM 2.5 measurements across NYC neighborhoods?
- How do SO2 emissions vary across different neighborhoods, and are there specific areas with significantly higher or lower emissions?
- What are the temporal trends in SO2 emissions in specific neighborhoods over the years?
- Are there noticeable seasonal patterns in PM 2.5 pollution levels?
- Which neighborhoods consistently show high levels of PM 2.5 and SO2 emissions?
# Data source and link
- NYC Air Quality Surveillance Data (Uploaded as Air_Quality_20240801.csv

# Challenge
This project aims to analyze the relationship between air quality indicators, such as PM 2.5 levels, and various health outcomes, including asthma emergency department visits, cardiovascular hospitalizations, and respiratory hospitalizations across different neighborhoods. We implemented both traditional statistical models (e.g., ARIMA) and deep learning models (e.g., Convolutional Neural Networks) to uncover correlations and make predictions based on historical data.

# Problem Statement
The primary objective of this project is to understand how air pollutants like PM 2.5 correlate with public health outcomes. Specifically, we aim to answer the following questions:

How do asthma emergency department visits correlate with fine particles (PM 2.5) in different neighborhoods?
What is the relationship between deaths due to PM2.5 and cardiovascular hospitalizations (age 40+) across NYC?
Analyze the correlation between respiratory hospitalizations (age 20+) and deaths due to PM 2.5.
Data Description
Data Sources
Air Quality Data: Provided by local environmental agencies, including measurements of pollutants like PM 2.5, NO2, O3, and SO2.
Health Outcomes Data: Sourced from public health records, including data on asthma emergency department visits, cardiovascular and respiratory hospitalizations.
Data Collection
Size of Data: The dataset includes several thousand records spanning multiple years.
Time Range: The data covers the period from 2005 to 2022.

# Solution Outline
Data Flow
Data Ingestion: The raw data is collected and pre-processed.
Data Transformation: The data is cleaned, normalized, and reshaped to be used in different models.
Data Storage: Processed data is stored locally for future reference and analysis.
Local Storage Layout

Raw Data: ../data/raw/

Processed Data: ../data/processed/

Notebooks: ../notebook/

# Data Preparation
Scaling and Encoding: The data values were scaled using MinMaxScaler to fit the range [0, 1]. Non-numerical columns were encoded as needed.
Feature Engineering: Additional columns such as 'Year' were derived from existing date columns.
Exploratory Analysis
Target Variable Distribution: Analyzed the distribution of key variables like PM 2.5 levels, asthma visits, etc.
Bivariate Analysis: Explored relationships between pollutants and health outcomes using scatter plots, correlation matrices, and time series plots.

# Modelling Experiment Design
Baseline Model
Custom CNN: Designed to predict future values of health outcomes based on historical pollutant data.
Hyperparameter Tuning: Conducted to optimize the model’s performance.
Model Evaluation
Metrics: Mean Squared Error (MSE) was used to evaluate model performance.
Comparison: The CNN model was compared against the ARIMA model, with the CNN showing superior performance in capturing complex patterns in the data.
Model Deployment
While the model is designed to be run in a Jupyter notebook, it can be deployed in a production environment where real-time data would be fed into the model for continuous predictions.

# Insights Reporting
Tableau Dashboard for Michael E https://public.tableau.com/app/profile/michael.elkabas/viz/Air_Quality-MichaelE/Dashboard1
A Tableau dashboard was created to visually explore and communicate the findings of the analysis.

# Limitations and Assumptions
Data Quality: The analysis assumes that the data is accurate and free from significant measurement errors.
Generalization: The models were trained on historical data and may not fully capture future trends due to changing environmental conditions.
Considerations for Future Work
Incorporate Real-Time Data: Integrate live data feeds to improve the model’s predictive capabilities.
Broader Geographic Scope: Extend the analysis to cover additional regions beyond NYC.

# Key Learnings
What Went Well: The CNN model demonstrated strong performance in capturing complex patterns in the data.
What Could Be Improved: Future work could focus on incorporating more advanced deep learning architectures or additional data sources.



