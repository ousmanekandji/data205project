## Ousmane Kandji
Food Inspection Outcomes and Closed Establishments Analysis
DATA 205 Capstone Report


## Introduction
This project analyzes food establishment inspection records and closure data to identify patterns related to public health risks and business closures. The purpose of the study is to understand common inspection outcomes, recurring violations, geographic differences, and trends over time.
## Datasets Used
1. FoodInspectionData.csv – contains general food inspection records.
2. Closed_Food_Establishments.csv – contains inspections that resulted in facility closure.

## Data Cleaning and Preparation
The datasets were cleaned in R using tidyverse packages. Duplicate rows were removed, city names were standardized, ZIP codes were converted to five-digit format, text spacing issues were fixed, and dates were converted into usable date formats. Missing values were identified and handled where necessary.

## Research Questions
•	What are the most common inspection outcomes?
•	What percentage of inspections resulted in closures?
•	Which violations appear most often in closure cases?
•	Are closures increasing or decreasing over time?
•	Which cities have the highest closure counts and closure rates?

## Methods
Exploratory Data Analysis (EDA) was performed using summary statistics and visualizations. Bar charts were used to compare inspection outcomes and violation frequencies. Line charts were used to evaluate monthly closure trends. City-level comparisons were made using closure counts and closure rates.

## Key Findings
•	Most inspections did not result in closure.
•	Closure events continued to occur across multiple months.
•	Temperature control, contamination, and sanitation violations appeared repeatedly in closure cases.
•	Some cities had higher closure rates relative to their total inspections.

## Limitations
The closure dataset is smaller than the full inspection dataset and may not represent every closure event. Some records may contain missing or inconsistently entered values. This analysis is descriptive and does not establish causation.

## Conclusion
This project demonstrates how public inspection data can be cleaned and analyzed to uncover useful food safety trends. The findings may help health departments focus prevention efforts, training, and enforcement in higher-risk areas.
