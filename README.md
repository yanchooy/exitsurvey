# Exitsurvey
An demographic analysis of dissatisfaction found in exit surveys from Department of Education, Training and Employment (DETE) and the Technical and Further Education (TAFE) institute in Queensland, Australia

# Goal
Are employees who only worked for the institutes for a short period of time resigning due to some kind of dissatisfaction? What about employees who have been there longer?

# Data inspection & Cleaning
    - Handling null values
    - Dropping irrelevant columns
    - Column names standardization for both datasets
    - Removing irrelevant values outside of scope
    - Verified the quality of our data by checking for inconsistencies in time period
    - Create a new dedicated column to aggregate employment period in both datasets
    - Create a new dedicated column populated with boolean values reflecting reason for resignation due to dissatisfaction in both datasets
    
# Data Transformation
    - Combining dataset through concatenation
    - Drop columns with null values higher than thresh parameter
    - Standardizing number of service years into categories i.e New, Established, Experienced, Veteran
    - Classifying age into age range i.e. less than 20, 21-30, 31-40, 41-50, 51-60, more than 60

# Data Analysis of people who are dissatisfied
    - Dissatisfaction by service category via pivot table and bar chart visualisation
    - Initial conclusion that longer working employees do not equate to higher resignations
    - Further analysis for dissatisfaction by age via pivot table and bar chart visualisation
    - Heatmap analysis of age and service years with dissatifaction percentage
![age_years_dissatisfied](https://github.com/yanchooy/exitsurvey/assets/109457905/cec55caa-bf79-4c50-9dcb-5db893316921)

# Conclusion
    - Conclusion of age and service years combined consideration
    - Employees who are between 41 - 50 years old who are veterans (more than 11 service years) are more likely to be dissatisfied with their jobs.
    - Low staff morale followed by salary dissatifaction are the top reasons for dissatisfaction for this group.
![disagree_factors](https://github.com/yanchooy/exitsurvey/assets/109457905/ee3a5ab2-6d0b-4e00-bfdb-6f93276d4a39)

