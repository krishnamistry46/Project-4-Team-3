Air Quality and Health Impact Analysis
Overview
This project explores the relationship between air quality indicators, specifically PM 2.5 levels, and various health outcomes such as asthma emergency department visits, cardiovascular hospitalizations, and respiratory hospitalizations in New York City. The analysis aims to provide insights into how air pollution correlates with adverse health effects across different neighborhoods.

Project Structure
Data Source: The dataset used in this analysis was sourced from various public health and environmental databases, covering a time range of several years. The dataset includes air quality indicators (PM 2.5, Ozone, SO2) and health outcome indicators (asthma emergency visits, cardiovascular hospitalizations, respiratory hospitalizations).

Data Processing and Modeling:

The data was pre-processed to handle missing values, normalize features, and generate new feature columns such as latitude and longitude.
Time series analysis and machine learning models (ARIMA and CNN) were applied to study trends and predict future outcomes based on historical data.
Visualization:

The results of the analysis were visualized using Tableau. A story was created in Tableau to present the findings, which includes:
The correlation between PM 2.5 levels and asthma emergency department visits.
The relationship between deaths due to PM 2.5 and cardiovascular hospitalizations (age 40+).
The correlation between respiratory hospitalizations (age 20+) and deaths due to PM 2.5.
The Tableau public visualization can be accessed here.

Usage
The Jupyter notebook analysis.ipynb contains all the steps for data processing, modeling, and generating visualizations.
The Tableau story can be viewed online using the provided link to explore the results interactively.
[https://public.tableau.com/authoring/Air_Quality-MichaelE/Story3#1](https://public.tableau.com/views/Air_Quality-MichaelE/Dashboard1?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)

Key Findings
Asthma Emergency Department Visits and Fine Particles (PM 2.5):

Correlation Coefficient: 0.9699
P-value: 0.0301
There is a strong positive correlation between PM 2.5 levels and asthma emergency visits, suggesting that higher PM 2.5 levels are strongly associated with more asthma emergencies.
Deaths due to PM 2.5 & Cardiovascular Hospitalizations (age 40+):

The analysis revealed a moderate positive correlation, indicating that increased PM 2.5 levels are associated with higher rates of cardiovascular hospitalizations.
Respiratory Hospitalizations (age 20+) and Deaths due to PM 2.5:

The results indicated a significant correlation, highlighting the impact of PM 2.5 on respiratory health.
Limitations
Data Granularity: The data used for this analysis may not capture all nuances at a more granular level, potentially impacting the accuracy of predictions.
Model Generalization: The CNN model may have limitations in generalizing to new, unseen data due to potential overfitting, requiring further validation and refinement.
Future Work
Incorporate Additional Data Sources: Including data on socioeconomic factors, healthcare access, and other pollutants could provide a more comprehensive analysis.
Model Refinement: Further tuning and experimenting with different machine learning models could improve prediction accuracy.

Project Analysis Questions:
1. What are the average, median, and variability of PM 2.5 measurements 
across NYC neighborhoods?
2. How do SO2 emissions vary across different neighborhoods, and are there 
specific areas with significantly higher or lower emissions?
3. What are the temporal trends in SO2 emissions in specific neighborhoods 
over the years?
4. Are there noticeable seasonal patterns in PM 2.5 pollution levels?
5. Which neighborhoods consistently show high levels of PM 2.5 and SO2 
emissions?
Data Source:
Dataset: NYC Air Quality Surveillance Data (Uploaded as 
Air_Quality_with_Coordinates.csv)
