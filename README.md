# Employee Churn Exploration

## Table of Contents

- [Project Overview](#project-overview)
- [Data Source](#data-source)
- [Tools](#tools)
- [Data Preprocessing](#data-preprocessing)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [Key Findings and Insights](#key-findings-and-insights)

## Project Overview
This project is designed to unravel the key factors influencing employee turnover within the organization. By leveraging data-driven techniques, our objective is to pinpoint the top features contributing to employee departures. The insights gained from this analysis will empower decision-makers to make informed strategic choices.

Goals:
- Identify the primary features correlated with employee turnover.
- Provide a comprehensive understanding of the workforce dynamics.
- Tailor recommendations based on the findings to mitigate employee turnover. </br>

Through a combination of exploratory data analysis, regression modeling, and clustering techniques, we aim to uncover patterns and trends that contribute to employee attrition. The ultimate goal is to equip stakeholders with actionable insights for fostering a more productive and satisfied workforce.

## Data Source
The department has assembled data on almost 10,000 employees. The team used information from exit interviews, performance reviews, and employee records.

> #### Features description:

- `department` - the department the employee belongs to.
- `promoted` - 1 if the employee was promoted in the previous 24 months, 0 otherwise.
- `review` - the composite score the employee received in their last evaluation.
- `projects` - how many projects the employee is involved in.
- `salary` - for confidentiality reasons, salary comes in three tiers: low, medium, high.
- `tenure` - how many years the employee has been at the company.
- `satisfaction` - a measure of employee satisfaction from surveys.
- `bonus` - 1 if the employee received a bonus in the previous 24 months, 0 otherwise. 
- `avg_hrs_month` - the average hours the employee worked in a month.
- `left` - "yes" if the employee ended up leaving, "no" otherwise.

## Tools
- Pandas: Data Cleaning - Exploratory Data Analysis
- Matplotlib: Data Visualization
- Seaborn: Data Visualization
- scikit-learn: Machine Learning Models

## Data Preprocessing
In the initial data preparation phase, we performed the following tasks:

1. **Data Loading and Inspection:**
   - Loaded the raw data into the analysis environment.
   - Conducted an initial inspection to understand the structure and content of the dataset.

2. **Handling Missing Values:**
   - Identified and addressed any missing values in the dataset.
   - Implemented strategies such as imputation or removal based on the nature and impact of missing data.

3. **Handling Outliers:**
   - Detected and addressed outliers that could potentially impact the analysis.
   - Applied appropriate techniques, such as statistical methods or visual inspection, to handle outliers.

4. **Handling Duplicate Values:**
   - Checked for and removed any duplicate records to ensure data integrity.
   - Resolved issues related to repeated entries that could affect the accuracy of the analysis.

5. **Data Cleaning and Formatting:**
   - Cleaned the data by addressing any inconsistencies or errors.
   - Formatted variables to ensure consistency and compatibility with the chosen analysis methods.

These preprocessing steps were essential to enhance the quality of the dataset and prepare it for subsequent exploratory and analytical phases.

## Exploratory Data Analysis (EDA)

EDA involved exploring the NBA All Seasons data to answer the following questions:

1. Which department has the highest employee turnover? Which one has the lowest?
2. Investigate which variables seem to be better predictors of employee departure.
3. What recommendations would you make regarding ways to reduce employee turnover?

## Key Findings and Insights:
### _**Which department has the highest employee turnover? Which one has the lowest?**_

In our examination of employee turnover, the Sales department emerged with the highest turnover, witnessing 537 departures. It was closely followed by the Retail and Engineering departments, with 471 and 437 departures, respectively. To gain deeper insights, we further scrutinized specific clusters based on employee characteristics.

- Balanced Performers
Within the "Balanced Performers" cluster, encompassing departments like Sales, Retail, and Operations, Sales continued to be a significant contributor to turnover, with 190 departures. Retail and Operations closely followed, recording 162 and 161 departures, respectively.

- High Review, Lower Satisfaction
In the cluster characterized by high review scores but lower satisfaction, Sales again stood out with the highest turnover, witnessing 231 departures. Retail and Engineering followed suit with 199 and 194 departures, respectively.

- Highly Satisfied, Moderate Performers
Exploring the cluster of highly satisfied employees with moderate performance, Sales maintained prominence with 116 departures. Retail and Operations also featured prominently, with 110 and 90 departures, respectively.

In summary, Sales consistently held the distinction of having the highest turnover across various clusters, closely trailed by Retail and Operations. While Engineering secured a spot in the top three overall, its ranking varied across different employee clusters.

### _**Investigate which variables seem to be better predictors of employee departure.**_

Our investigation into predictor variables unveiled critical insights. Performance review scores (review) emerged as the most consistent and influential predictor in both linear and logistic regression models. It consistently held the top position across different employee clusters, highlighting its robust association with employee departures. Additionally, average monthly hours worked (avg_hrs_month) demonstrated significance, securing the second and third positions in linear and logistic regression, respectively. Job satisfaction (satisfaction) consistently appeared among the top three predictors, emphasizing its role in influencing employee turnover.

### _**What recommendations would you make regarding ways to reduce employee turnover?**_

While the ideal turnover rate is generally considered to be 10% or lower for maintaining a stable labor force, our analysis uncovered a higher-than-average turnover rate of around 30%. This indicates a critical need for strategic interventions to address employee retention. The breakdown across different clusters and departments provides valuable insights for tailoring recommendations.

**Overall Strategy:**
The company should focus on implementing a comprehensive employee retention strategy, addressing key factors influencing turnover. A holistic approach should include measures to enhance job satisfaction, provide growth opportunities, and recognize and reward high performers.

> **Balanced Performers:**

- `Identify and Acknowledge High Performers:` Recognize and reward employees in the Sales, Retail, and Operations departments for their contributions.
- `Promotions and Bonuses:` Increase the annual promotions rate and consider introducing additional bonuses for outstanding performance.
- `Career Development:` Establish clear career progression paths and communicate growth opportunities within the organization.
- `Enhanced Benefits:` Review and enhance benefits packages, considering factors beyond monetary compensation.

> **High Review, Lower Satisfaction:**

- `Performance-Linked Incentives:` Implement performance-linked incentives, such as performance-based bonuses and promotions.
- `Satisfaction Surveys:` Conduct regular satisfaction surveys to understand and address specific concerns affecting job satisfaction.
- `Work-Life Balance:` Explore initiatives to improve work-life balance, considering the impact of working hours on employee satisfaction.
- `Leadership Development:` Provide leadership development programs to enhance the skills and satisfaction of employees in Engineering, Sales, and Retail.

> **Highly Satisfied, Moderate Performers:**

- `Recognition Programs:` Implement employee recognition programs to acknowledge the efforts of highly satisfied employees.
- `Performance-Driven Rewards:` Introduce rewards aligned with performance metrics to motivate moderate performers.
- `Training Opportunities: Offer training opportunities to enhance the skills and capabilities of employees in Sales, Retail, and Operations.
- `Flexible Working Conditions:` Consider flexible working arrangements to accommodate the preferences of highly satisfied employees.

> **Company-Wide Initiatives:**

- `Meritocracy System:` Establish a robust meritocracy system to ensure that promotions and rewards are based on performance and contributions.
- `Communication Channels:` Enhance communication channels to keep employees informed about organizational developments and opportunities.
- `Regular Feedback:` Implement regular feedback mechanisms to address concerns and proactively identify areas for improvement.
- `Competitive Salaries:` Regularly review and adjust salary structures to remain competitive in the industry.
