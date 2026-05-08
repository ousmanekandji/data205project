## Ousmane Kandji
Food Inspection Outcomes and Closed Establishments Analysis
DATA 205 Capstone Report


# Project Overview

Food inspection records show that most establishments pass inspections, but closures and failed inspections still occur due to recurring critical violations. This project investigates patterns in food safety enforcement by analyzing inspection outcomes, closure-related violations, and geographic differences in closure activity across cities.

The main questions this project investigates are:

What inspection outcomes are most common?

Which critical violations appear most frequently in closure cases?

Are failed inspections associated with critical violations?

Do critical violations increase the likelihood of closure outcomes?

Which cities experience higher closure activity and closure rates?

To answer these questions, two food inspection datasets were cleaned, standardized, and analyzed in R using exploratory data analysis and statistical methods. The project combines descriptive visualization with chi-square testing and logistic regression to better understand relationships between inspection outcomes and critical violations.

# Datasets Used

FoodInspectionData.csv

Contains general inspection records for food establishments
Includes inspection outcomes, inspection dates, business locations, and critical violation indicators
Used as the primary dataset for cleaning, exploratory analysis, and statistical testing
Closed_Food_Establishments.csv

Contains inspections associated with facility closure events
Used to analyze common violations among closed establishments
Used to examine closure trends over time
Provides a more focused view of high-risk inspections
Together, the datasets provide both a broad overview of inspection activity and a focused look at closure-related public health concerns.

# Tools Used

R was used for all data cleaning, analysis, statistical testing, and visualization.

Main libraries used:

tidyverse

ggplot2

lubridate

knitr

# Data Cleaning

Several cleaning steps were needed before analysis:

Removed duplicate inspection rows

Standardized ZIP codes and city names

Converted inspection dates into date format

Created the is_closed variable

Created the critical_count variable

Standardized violation language across datasets

Exported cleaned datasets for analysis

The final cleaned datasets allowed inspection outcomes, closure events, and critical violations to be analyzed consistently across both datasets.

# Analysis

The exploratory analysis looked at:

Inspection outcome distributions

Most common violations among closure inspections

Monthly closure trends

Top cities by closure count

City-level closure rates

One important metric used in the project was critical_count, which measures the number of critical violations found during an inspection. This helped compare inspections by overall violation severity rather than individual violations alone.

The project also examined whether failed inspections were associated with critical violations and whether higher numbers of critical violations increased the likelihood of closure outcomes.

# Final Statistical Analysis

The final statistical analysis included:

Chi-square testing

Logistic regression

The chi-square test was used to determine whether inspection outcomes were associated with the presence of critical violations.

The logistic regression model used was:

is_closed ~ critical_count

Where:

is_closed = whether an inspection resulted in a closure outcome

critical_count = number of critical violations during the inspection

Why This Analysis Was Used

This analysis helps evaluate whether critical violations are related to failed inspections and increased closure risk.

Instead of only describing inspection outcomes, the project also tests whether higher numbers of critical violations are statistically associated with more serious inspection outcomes.

# Model Results

The chi-square analysis showed that failed inspections were more likely to contain critical violations than passed inspections.

The logistic regression model showed that higher critical violation counts were associated with increased odds of closure outcomes.

The results support the idea that recurring critical violations are strong indicators of higher food safety risk.

# Key Findings

Most inspections result in a pass

Closure outcomes are relatively rare compared to total inspections

Closure events still occur consistently over time

Several critical violations repeatedly appeared in closure-related inspections

Violations related to temperature control, contamination, sanitation, and water availability appeared frequently in closure cases

Some cities showed higher closure activity and closure rates than others

Food safety risk was not evenly distributed geographically

# Conclusion

This project demonstrates how food inspection datasets can be cleaned, organized, visualized, and statistically analyzed to better understand food safety risks and closure patterns.

The findings show that recurring critical violations are associated with more serious inspection outcomes and increased closure risk. Overall, the project highlights how inspection data can support public health monitoring and help identify higher-risk food establishments and locations.
