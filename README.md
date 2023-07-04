# Exitsurvey
An demographic analysis of dissatisfaction found in exit surveys from Department of Education, Training and Employment (DETE) and the Technical and Further Education (TAFE) institute in Queensland, Australia

# Goal
Are employees who only worked for the institutes for a short period of time resigning due to some kind of dissatisfaction? What about employees who have been there longer?

# Table of Contents
## Introduction to dataset and analysis goals
## Data inspection
## Data Cleaning
    - Handling null values
    - Dropping irrelevant columns
    - Column names standardization for both datasets
    - Removing irrelevant values outside of scope
    - Verified the quality of our data by checking for inconsistencies in time period
    - Create a new dedicated column to aggregate employment period in both datasets
    - Create a new dedicated column populated with boolean values reflecting reason for resignation due to dissatisfaction in both datasets
## Data Transformation
    - Combining dataset through concatenation
    - Drop columns with null values higher than thresh parameter
    - Standardizing number of service years into categories i.e New, Established, Experienced, Veteran
    - Classifying age into age range i.e. less than 20, 21-30, 31-40, 41-50, 51-60, more than 60

## Data Analysis of people who are dissatisfied
    - Dissatisfaction by service category via pivot table and bar chart visualisation
    - Initial conclusion if service years lead to higher dissatisfaction
    - Dissatisfaction by age via pivot table and bar chart visualisation
    - Heatmap analysis of age and service years with dissatifaction percentage
    - Conclusion of age and service years combined consideration
    - Push factors for dissatisfaction
# Conclusion
