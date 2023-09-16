# IBM HR Analytics Employee Attrition & Performance Analysis
## Overview

This Jupyter Notebook project focuses on a comprehensive analysis of employee attrition and performance using the [IBM HR Analytics dataset](https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset). The dataset contains 1470 records and 35 columns, with no missing values. It encompasses 26 numerical and 9 categorical columns. Some columns, such as 'EmployeeCount', 'EmployeeNumber', 'Over18', and 'StandardHours,' have been excluded from the analysis due to their lack of relevance.

## Dataset Details

The [IBM HR Analytics dataset](https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset) offers a rich source of information about employees within an organization. Here are key columns and their descriptions:

- **Age:** Employee's age, providing insights into workforce demographics.
- **Attrition:** A binary indicator (Yes/No) of whether the employee has left the company (target variable).
- **BusinessTravel:** Frequency of business travel undertaken by employees, which can affect job satisfaction and attrition rates.
- **DailyRate:** The daily rate of pay for each employee, a critical compensation metric.
- **Department:** Indicates the specific department or division within the company where the employee works.
- **DistanceFromHome:** Reflects the distance in miles between the employee's home and the workplace, a factor related to commuting and job satisfaction.
- **Education:** Specifies the education level attained by employees, influencing career prospects and job satisfaction.
- **EducationField:** Describes the field or specialization of education for each employee, providing insights into qualifications.
- **EnvironmentSatisfaction:** Measures employee satisfaction with their work environment, impacting overall job satisfaction and retention.
- **Gender:** Indicates the gender of each employee, relevant for diversity and inclusion analysis.
- **HourlyRate:** The hourly rate of pay for employees, crucial for assessing compensation structures.
- **JobInvolvement:** Reflects the level of job involvement of each employee, indicating engagement.
- **JobLevel:** Specifies the job level or rank of each employee within the organization.
- **JobRole:** Describes the specific role or position held by each employee in the company.
- **JobSatisfaction:** Measures overall job satisfaction among employees.
- **MaritalStatus:** Indicates the marital status of employees, related to life stage considerations and job mobility.
- **MonthlyIncome:** Specifies the monthly income earned by each employee, a key financial factor.
- **MonthlyRate:** The monthly rate of pay for employees, complementing the compensation picture.
- **NumCompaniesWorked:** Indicates the number of different companies for which each employee has previously worked, potentially linked to attrition trends.
- **OverTime:** A binary indicator (Yes/No) revealing whether the employee works overtime, offering insights into work-life balance.
- **PercentSalaryHike:** Reflects the percentage increase in salary for employees, a key compensation metric.
- **PerformanceRating:** Specifies employee performance ratings, essential for understanding performance-related factors.
- **RelationshipSatisfaction:** Measures employee satisfaction with workplace relationships, crucial for assessing team dynamics.
- **StockOptionLevel:** Indicates the level of stock options held by each employee, a valuable compensation component.
- **TotalWorkingYears:** Specifies the total number of years of work experience for each employee.
- **TrainingTimesLastYear:** Reflects the number of training sessions attended by employees in the last year, relevant for skill development.
- **WorkLifeBalance:** Measures satisfaction with work-life balance, an important factor in job retention.
- **YearsAtCompany:** Indicates the number of years each employee has spent at the current company.
- **YearsInCurrentRole:** Specifies the number of years each employee has spent in their current role.
- **YearsSinceLastPromotion:** Reflects the number of years since the last promotion for each employee.
- **YearsWithCurrManager:** Indicates the number of years each employee has worked with their current manager.

This comprehensive dataset provides a wealth of information for analyzing employee attrition, job performance, and the factors that influence them.

## Data Exploration

The analysis includes visualizations to gain insights into attrition and its relationship with various factors:

- **Attrition by Age:** A count plot illustrating attrition by age.
- **Attrition by Business Travel:** A count plot showing attrition by business travel frequency.
- **Attrition by Department:** A count plot depicting attrition by department.
- **Attrition by DistanceFromHome:** A count plot demonstrating attrition by distance from home.
- **Attrition for Other Columns:** Count plots for other pertinent columns.

## Data Preprocessing

To prepare the data for analysis, the `wrangle` function has been employed. This function handles tasks such as encoding categorical variables and mapping binary categories. Additionally, feature selection and engineering have been carried out.

## Modeling

Four different models have been implemented and evaluated to predict employee attrition:

1. **Logistic Regression (LR):** A logistic regression model.
2. **Random Forest (RF):** A random forest classifier.
3. **Decision Tree (DT):** A decision tree classifier.
4. **K-Nearest Neighbors (KNN):** A k-nearest neighbors classifier.

Each model's performance has been cross-validated, and accuracy scores are reported.

## Model Tuning

To optimize the models, hyperparameter tuning has been performed on the Random Forest (RF) and Logistic Regression (LR) models using GridSearchCV.

## Feature Importance

A bar plot visualizes the top 10 features that are most important in predicting attrition.

## Usage

To run this Jupyter Notebook project:

1. Install the necessary Python libraries (Pandas, NumPy, Matplotlib, Seaborn, Scikit-Learn) if not already installed.
2. Download the [IBM HR Analytics dataset](https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset) and place it in the same directory as this notebook.
3. Execute the code cells in this notebook in sequential order.
## Conclusion

In this comprehensive analysis of employee attrition and performance using the [IBM HR Analytics dataset](https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset), we've gained valuable insights into the factors influencing attrition within the organization. Here are some key takeaways:

- **Age and Attrition:** We observed that attrition tends to be higher among younger employees. This may suggest that the organization should focus on strategies to retain and engage younger talent.

- **Business Travel and Attrition:** Employees who travel frequently for business are more likely to experience attrition. This highlights the need to address the challenges faced by frequent travelers.

- **Department and Attrition:** The department in which an employee works plays a significant role in attrition rates. Identifying departments with higher attrition rates can help in targeted interventions.

- **Work-Life Balance:** Employees with better work-life balance tend to stay longer with the company. Encouraging and facilitating work-life balance could be a key strategy for reducing attrition.

- **Modeling:** We built and evaluated four different models (Logistic Regression, Random Forest, Decision Tree, K-Nearest Neighbors) to predict attrition. The Random Forest model showed the highest accuracy.

- **Feature Importance:** The top 10 features most important in predicting attrition were identified. This information can guide HR strategies by focusing on key factors affecting attrition.

## Next Steps

This analysis serves as a foundation for making data-driven HR decisions to reduce attrition rates and enhance employee performance. Some potential next steps include:

- Implementing retention strategies tailored to specific age groups and departments.
- Offering solutions to address the challenges faced by employees who travel frequently.
- Conducting surveys or interviews to gather qualitative data for a deeper understanding of employee needs and concerns.
- Continuously monitoring and analyzing attrition rates to adapt strategies over time.

By taking proactive steps based on the insights from this analysis, the organization can foster a more engaged and satisfied workforce, ultimately contributing to its long-term success.

