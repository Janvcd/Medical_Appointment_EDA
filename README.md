# Medical Appointment Data Analysis

## Overview

This project analyzes a medical appointment dataset using a Jupyter Notebook (`Medical_Appointment_Data.ipynb`). The goal is to understand patient behavior and identify factors affecting attendance at medical appointments. The analysis involves data cleaning, feature engineering, and visualization.

## Dataset

The dataset used in this analysis is `Medical_data.csv`, which includes patient demographics, medical history, appointment details, and attendance records.

## Key Findings

- More female patients attend appointments compared to male patients.
- The "NoShow" and "Show" ratio remains nearly equal across most age groups, except for infants (Age 0 and 1), where 80% attended.
- Most neighborhoods exhibit an 80% appointment attendance rate.
- Patients without a scholarship had an 80% attendance rate, while those with a scholarship had a 75% attendance rate.
- 85% of patients with hypertension attended, compared to 78% of those without hypertension.
- 83% of diabetic patients attended, compared to 80% of non-diabetic patients.
- 84% of patients who did not receive an SMS reminder attended, while only 72% of those who received an SMS did.
- Appointments are not scheduled on Sundays, and there are fewer appointments on Saturdays compared to weekdays.

## Dependencies

The following Python libraries are required:

```bash
pip install pandas numpy matplotlib seaborn
```

## Data Processing Steps

1. **Loading the dataset:** Using `pandas.read_csv()` to load `Medical_data.csv`.
2. **Data Cleaning:**
   - Converting date columns (`ScheduledDay`, `AppointmentDay`) to `datetime` format.
   - Renaming columns for consistency.
3. **Feature Engineering:**
   - Extracting weekday information from date columns.
   - Creating dummy variables for categorical data.
4. **Exploratory Data Analysis (EDA):**
   - Examining the distribution of `NoShow` across different variables.
   - Visualizing trends using bar charts and histograms.

## How to Run

1. Clone this repository or download the notebook.
2. Install the required dependencies.
3. Open the Jupyter Notebook:
   ```bash
   jupyter notebook Medical_Appointment_Data.ipynb
   ```

## Visualizations

The notebook contains various visualizations that analyze patient attendance trends based on factors such as age, gender, medical conditions, and SMS reminders.

## Conclusion

This analysis provides insights into factors affecting patient attendance at medical appointments. The findings can help improve scheduling strategies and reduce no-show rates.
