🏥 Healthcare Appointment No-show Analysis
This project investigates the factors contributing to patients missing their scheduled medical appointments. By analyzing a dataset of over 110,000 records from Brazil, we aim to identify patterns and develop insights that could help healthcare providers reduce no-show rates and optimize scheduling strategies.

📁 Dataset Overview
Source: Kaggle - Medical Appointment No Shows

Filename: KaggleV2-May-2016.csv

Records: 110,527

Features: 14 attributes including:

Patient ID

Appointment ID

Scheduled Date

Appointment Date

Age, Gender

Neighbourhood

SMS Received

Health Conditions: Hypertension, Diabetes, Alcoholism, Handicap

Scholarship (indicates enrollment in welfare program)

No-show indicator

🎯 Project Objectives
Clean and preprocess real-world healthcare appointment data.

Perform exploratory data analysis (EDA) to understand patient behavior.

Identify key drivers for missed appointments.

Create visual dashboards using Power BI for business insights.

Suggest practical recommendations for reducing no-show rates.

🧰 Tools & Technologies Used
Tool	Purpose
Python	Data wrangling, EDA
Pandas	Data manipulation
NumPy	Numeric operations
Seaborn / Matplotlib	Data visualization
Power BI	Interactive dashboard & reports
Jupyter Notebook	Code execution & documentation

🔄 Data Preprocessing Steps
Converted ScheduledDay and AppointmentDay to datetime format.

Created a new feature WaitingDays = AppointmentDay - ScheduledDay.

Filtered out rows with negative WaitingDays.

Converted No-show column from Yes/No to binary (1 = No-show, 0 = Show).

Removed duplicate rows (if any).

Checked for and confirmed absence of missing values.

Extracted additional features like AppointmentWeekDay for weekday analysis.

📊 Exploratory Data Analysis (Key Findings)
1. Gender
Females had more appointments than males.

No significant difference in no-show rates between genders.

2. Age
Younger patients (especially 0–20 years) are more likely to miss appointments.

Older individuals (>60 years) have higher attendance rates.

3. SMS Reminders
Nearly 50% of patients received SMS reminders.

Surprisingly, the no-show rate was slightly higher among those who received an SMS, suggesting reminders alone aren't sufficient.

4. Weekday Patterns
Most appointments are scheduled Monday–Friday.

No-shows increase slightly on Fridays — possibly due to weekend proximity or fatigue.

5. Medical Conditions
Patients with hypertension and diabetes tend to show up more regularly.

Alcoholism and handicap status do not significantly impact attendance.

6. Waiting Days
Shorter wait times between scheduling and appointment result in higher attendance.

As WaitingDays increases, so does the likelihood of no-shows.

7. Neighborhood Analysis
Appointment attendance varies by neighborhood.

Some areas (e.g., JARDIM CAMBURI, MARIA ORTIZ) show better adherence than others, implying potential socio-economic influences.

📊 Power BI Dashboard Insights
The Power BI report includes:

Appointment and no-show counts segmented by gender, age group, health conditions, and weekday.

WaitingDays impact on no-shows using histogram.

Top 10 neighborhoods with visualized attendance behavior.

Interactive filters for deep dive exploration.

✅ Conclusion
There is no single dominant factor predicting no-shows.

A combination of variables — especially age, waiting days, medical conditions, and neighborhood — influences attendance.

Behavioral, social, and economic factors must be considered to create effective intervention strategies.

Further steps could involve predictive modeling (e.g., logistic regression, decision trees) to forecast patient attendance.

