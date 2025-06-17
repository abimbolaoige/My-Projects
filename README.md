# My-Projects
### Python Projects
#### Mini Project 1

#### Mini Project 2

#### Mini Project 3
###### Titanic Data Analysis Project Summary
This project explores the famous Titanic passenger dataset, focusing on uncovering patterns related to survival, passenger demographics, and boarding details using Python libraries like Pandas, Matplotlib, and Seaborn.

#### Key Tasks and Insights
##### 1.	Data Preparation:
* Loaded a CSV file where data was initially stored in a single comma-separated column.
* Split the column into multiple columns for structured analysis.
* Cleaned and converted appropriate data types (e.g., age, fare as float).
##### 2.	Survival Analysis:
* Calculated overall survival rate.
* Compared survival rates by passenger class (pclass), gender, and embarkation point.
##### 3.	Data Visualization:
* Created a histogram of passenger ages, labeling each bar with percentage values.
* Used bar plots to show embarkation counts and total numbers.
* Emphasized percentage distribution for better interpretability.
##### 4.	Error Handling and Debugging:
* Resolved errors due to incorrect column names and data types.
* Handled KeyError and TypeError from misformatted data during analysis.
##### 5.	Embarkation Analysis:
* Counted passengers by embarkation points (S, C, Q).
* Summarized total number of passengers who boarded the ship.

#### Key Analysis
##### Survival Analysis
##### 1. Overall Survival Rate:
* The survival rate was approximately 38–40%, meaning more than half of the passengers did not survive.
##### 2. By Passenger Class (pclass):
* 1st Class: Highest survival rate (~62%).
* 2nd Class: Moderate survival rate (~47%).
* 3rd Class: Lowest survival rate (~24%).
###### Insight: Higher-class passengers had significantly better survival chances.

##### By Gender (sex):
* Female Survival Rate: Very high (~74%).
* Male Survival Rate: Very low (~19%).
###### Insight: Women were prioritized during rescue operations (“women and children first”).

##### Age Distribution
* The age range of passengers varied from infants to elderly (0–80+ years).
* Majority of passengers were between 20 to 40 years.
* A histogram showed:
*     A peak around age 25–30.
*     Few very young or very old passengers.
###### Insight: The Titanic carried mostly young to middle-aged adults

##### Embarkation Analysis (embarked)
###### Embarkation Points:
* S (Southampton): Majority boarded here (~72%).
* C (Cherbourg): ~19% of passengers.
* Q (Queenstown): ~9% of passengers.
* No Categorization: 0.
###### Total Embarked Passengers: Sum of all 3 locations.
###### Insight: Southampton was the main departure port

##### Visualization Enhancements
* The age histogram was modified to:
- Show percentage of passengers in each age bin.
- Include labels above each bar for clarity.
* Bar plots for embarked included counts and total representation

##### Conclusion
Survival:      Higher in 1st class, women, and children.
Age:	         Most passengers were young adults.
Embarkation:   Majority of passengers boarded at Southampton.
Gender Gap:    Clear disparity in survival based on gender (women favored).
Class Divide:  Wealth/class directly influenced survival odds.




