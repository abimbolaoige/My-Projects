# My-Projects
### Python Projects
### Mini Project 1

### Mini Project 2

### Telecom Churn Analysis – Mini Project 2

### Project Overview

This project focuses on analyzing a telecom dataset to understand **customer churn behavior**. The goal is to identify patterns and factors associated with customer retention and churn using **Python** data analysis and visualization libraries.


### 🛠Tools & Libraries Used

```python
import pandas as pd
import numpy as np
import seaborn as sns
import matplotlib.pyplot as plt
```

### Data Loading & Exploration

```python
# Load the dataset
data = pd.read_csv('telecom_churn.csv')

# Basic info and structure
print("Shape of the DataFrame:", data.shape)
data.info()
print(data.describe())
```

### Data Preprocessing

```python
# Convert 'Churn' column from boolean to integer
data['Churn'] = data['Churn'].astype('int64')
print(data.info())
```

### Churn Distribution

```python
# Count churned vs non-churned customers
churn_counts = data['Churn'].value_counts().rename(index={0: 'Not Churned', 1: 'Churned'})

# Plot the distribution
churn_counts.plot(kind='bar', color=['green', 'red'])
plt.title('Churn Distribution')
plt.ylabel('Number of Customers')
plt.xlabel('Churn Status')
plt.xticks(rotation=0)
plt.grid(axis='y', linestyle='--', alpha=0.7)
plt.show()
```

### Churn Proportion

```python
# Calculate churn rate
churn_proportion = data['Churn'].mean()
print(f"Proportion of churned users: {churn_proportion:.4f} ({churn_proportion*100:.2f}%)")
```

### Sample Data View

```python
# View first 5 rows and first 3 columns
print(data.iloc[:5, :3])
```

### Key Takeaways

* The dataset was explored to understand structure and customer behavior.
* Visualizations highlighted the proportion and distribution of churned customers.
* This sets the stage for deeper analysis like feature importance, correlation, and predictive modeling.


### File Structure (Example)

```
├── telecom_churn.csv
├── telecom_churn_analysis.ipynb
└── README.md
```


### Mini Project 3
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
###### Total Embarked Passengers: Sum of all locations.
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




