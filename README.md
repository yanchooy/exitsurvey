# Exitsurvey

# Introduction
An demographic analysis of dissatisfaction found in exit surveys from Department of Education, Training and Employment (DETE) and the Technical and Further Education (TAFE) institute in Queensland, Australia. The original TAFE exit survey data is no longer available. Some slight modifications were made to the original datasets to make them easier to work with, including changing the encoding to UTF-8 (the original ones are encoded using cp1252.)
[DETE](https://data.gov.au/dataset/ds-qld-fe96ff30-d157-4a81-851d-215f2a0fe26d/details?q=exit%20survey) dataset contains 822 rows and 56 columns while 
TAFE dataset contains 702 rows and 72 columns.

# Goal
Are employees who only worked for the institutes for a short period of time resigning due to some kind of dissatisfaction? 
What about employees who have been there longer?

Below is a preview of a couple columns we'll work with from the `dete_survey.csv`:

* `ID`: An id used to identify the participant of the survey
* `SeparationType`: The reason why the person's employment ended
* `Cease Date`: The year or month the person's employment ended
* `DETE Start Date`: The year the person began employment with the DETE

Below is a preview of a couple columns we'll work with from the `tafe_survey.csv`:

* `Record ID`: An id used to identify the participant of the survey
* `Reason for ceasing employment`: The reason why the person's employment ended
* `LengthofServiceOverall. Overall Length of Service at Institute (in years)`: The length of the person's employment (in years)
  
# Conclusion
- Employees who are between 41 - 50 years old who are veterans (more than 11 service years) are more likely to be dissatisfied with their jobs.
- Low staff morale followed by salary dissatifaction are the top reasons for dissatisfaction for this group.
    
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

- Heatmap analysis of age and factors of dissatisfaction
  
![disagree_factors](https://github.com/yanchooy/exitsurvey/assets/109457905/ee3a5ab2-6d0b-4e00-bfdb-6f93276d4a39)

