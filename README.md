# 🏥 Healthcare Appointment No-show Analysis

This project analyzes a real-world medical appointment dataset from Brazil to identify patterns and factors contributing to patients missing their scheduled appointments. Through data preprocessing, exploratory data analysis (EDA), and dashboard visualizations, we aim to generate insights that could help healthcare providers reduce no-shows and optimize their scheduling systems.
---

## 🎯 Project Objectives

- Clean and preprocess medical appointment data.
- Perform EDA to understand patient behavior and trends.
- Visualize insights using Python and Power BI.
- Identify key factors influencing no-show behavior.
- Recommend strategies to reduce missed appointments.

---

## 🧰 Tools & Technologies

- **Python** (Pandas, NumPy, Matplotlib, Seaborn)
- **Jupyter Notebook**
- **Power BI Desktop**
- **Markdown** for documentation

---

## 🔄 Data Preprocessing Steps

- Converted date fields (`ScheduledDay`, `AppointmentDay`) to datetime format.
- Created new feature `WaitingDays = AppointmentDay - ScheduledDay`.
- Filtered out rows with negative waiting days.
- Converted `No-show` column from `"Yes"/"No"` to binary `1/0`.
- Removed duplicate rows.
- Created `AppointmentWeekDay` column for weekday-based analysis.

---

## 📊 Exploratory Data Analysis (Key Findings)

### ✅ Gender
- More appointments were scheduled by females.
- No significant difference in no-show rates between genders.

### ✅ Age
- Younger patients (<20) have higher no-show rates.
- Older individuals (>60) are more consistent in showing up.

### ✅ SMS Reminders
- Nearly 50% of patients received reminders.
- Patients who received SMS were **slightly more likely** to miss appointments.

### ✅ Weekday Trends
- Most appointments are scheduled Mon–Fri, with peak on Wednesday.
- Slight increase in no-shows on Fridays.

### ✅ Medical Conditions
- Patients with hypertension and diabetes were more likely to attend.
- No significant difference with alcoholism or handicap.

### ✅ Waiting Time
- No-shows increase with longer waiting periods between scheduling and appointment day.

### ✅ Neighborhoods
- Certain neighborhoods show better attendance rates.
- Socio-economic conditions may impact patient reliability.

---

## 📈 Power BI Dashboard

The interactive Power BI dashboard includes:

- Appointment volumes by:
  - Gender
  - Age Group
  - Weekday
  - Neighborhood
- No-show rates by:
  - Health Conditions
  - SMS Received
  - Waiting Days
- Filters to explore dimensions and correlations

> 📎 Files: See `HEALTH CARE PROJECT.pdf` for Power BI visual snapshots

---

## ✅ Conclusions

- There’s no single factor that determines no-show behavior.
- A combination of age, health condition, waiting time, and neighborhood influences attendance.
- SMS reminders alone may not be effective — a more integrated patient engagement strategy is needed.

---

## 🚀 Future Work

- Develop predictive models (e.g., logistic regression, decision trees) to forecast no-shows.
- Include external data like weather or transport for richer context.
- Deploy an interactive web-based dashboard using Streamlit or Flask.

---

## 📂 Project Files

| File Name                               | Description                                    |
|----------------------------------------|------------------------------------------------|
| `vertopal.com_Healthcare Appointment.pdf` | Python EDA, preprocessing, and visualizations |
| `HEALTH CARE PROJECT.pdf`              | Power BI dashboards & business insights       |

