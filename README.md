## Ousmane Kandji
Food Inspection Outcomes and Closed Establishments Analysis
DATA 205 Capstone Report


# Project Overview
Food inspection records show that most establishments pass inspections, but closures still occur consistently over time due to recurring violations. This project investigates what drives those closures by asking: what inspection outcomes are most common, which violations appear most frequently in closure cases, and whether certain cities experience higher closure risk than others. To answer this, I worked with two datasets, cleaned and standardized them in R, performed exploratory data analysis, and examined patterns across time and location to better understand food safety risks.

# Datasets Used
The first dataset, FoodInspectionData.csv, contains general inspection results for food establishments and is used to analyze overall inspection outcomes and trends. The second dataset, Closed_Food_Establishments.csv, focuses specifically on inspections that resulted in facility closures, allowing for deeper analysis of high-risk violations and closure patterns. Together, these datasets provide both a broad and focused view of food safety enforcement.

# Tools Used in This Project
All analysis was performed in R, using the tidyverse for data manipulation and cleaning, lubridate for handling dates, and ggplot2 for visualization. These tools were used to transform raw inspection records into meaningful insights through structured analysis and clear visual representation.

# Analysis
The exploratory data analysis examines inspection outcomes, violation frequencies, and closure trends over time. Bar charts are used to compare inspection results and identify the most common violations among closed establishments, while line charts track how closures change month to month. A key part of the analysis is comparing cities by both total closure counts and relative closure rates, which provides a better understanding of risk beyond just raw numbers.
The analysis focuses on identifying patterns rather than building predictive models. By combining inspection data with closure-specific records, the project highlights which violations are most associated with shutdowns and how those risks vary across different locations.

# Key Findings
The results show that most inspections result in a pass, meaning closures are relatively rare compared to total inspections. However, closure events still occur consistently over time, indicating ongoing public health concerns. A small number of violations appear repeatedly in closure cases, particularly those related to temperature control, food contamination, and sanitation. These issues are strong indicators of higher risk. Additionally, some cities have higher closure rates relative to their total number of inspections, suggesting that risk is not evenly distributed geographically.

# Limitations
The closure dataset is significantly smaller than the full inspection dataset and may not capture every closure event. Some records may also contain missing or inconsistently formatted values, which can affect accuracy. This analysis is descriptive and does not establish causal relationships between violations and closures.

# Conclusion
This project demonstrates how food inspection data can be cleaned, organized, and analyzed to uncover meaningful patterns in public health and safety. By identifying recurring violations and geographic differences in closure risk, the findings can help inform better targeting of inspections, training, and prevention efforts.
