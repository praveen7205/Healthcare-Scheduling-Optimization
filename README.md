
# 🏥 Healthcare Appointment No-Show Prediction

Predicting whether a patient will miss their scheduled medical appointment and providing data-driven insights to help healthcare providers optimize scheduling and reduce missed appointments.

---

## 📌 Project Overview

This project analyzes historical patient appointment data to:
- Predict the likelihood of a patient not showing up
- Identify key trends (age, weekday, SMS reminders)
- Visualize insights via a Power BI dashboard
- Recommend strategies to reduce no-shows

---

## 🧰 Tools & Technologies

- **Python**: Data cleaning, feature engineering, machine learning (Pandas, Scikit-learn)
- **Power BI**: Dashboard for visual analytics
- **Decision Tree Classifier**: For classification modeling

---

## 📁 Dataset

- **Source**: [Kaggle - Medical Appointment No Shows](https://www.kaggle.com/datasets/joniarroba/noshowappointments)
- **Columns include**:
  - `Gender`, `Age`, `Scholarship`, `Hipertension`, `Diabetes`, `Alcoholism`, `Handcap`
  - `ScheduledDay`, `AppointmentDay`
  - `SMS_received`, `No-show`

---

## 🔄 Project Workflow

1. **Data Cleaning**
   - Converted date columns to datetime
   - Calculated waiting days
   - Filtered invalid records
   - Replaced gender values with full names

2. **Feature Engineering**
   - Created `Weekday`, `WaitingDays`, and `AgeGroup` columns
   - Encoded categorical features

3. **Modeling**
   - Trained a Decision Tree Classifier
   - Evaluated with accuracy, confusion matrix, and classification report
   - Added model predictions to the dataset

4. **Power BI Dashboard**
   - Visualized no-show trends, prediction insights, and behavior by gender, age, SMS, and weekday
   - Included filters for dynamic exploration

---

## 📊 Power BI Dashboard Features

- **KPIs**: Total appointments, % No-shows, Model Accuracy
- **Charts**:
  - No-shows by weekday and gender
  - SMS reminder impact
  - Age group risk levels
  - Prediction vs Actual comparison table
  - Neighborhood no-show rates (map/table)
- **Slicers**: Gender, AgeGroup, SMS, Weekday, Prediction

> 📍 The Power BI `.pbix` file is included in this repository.

---

## 📦 Files Included

| File Name                             | Description                                 |
|--------------------------------------|---------------------------------------------|
| `KaggleV2-May-2016.csv`              | Original dataset                            |
| `no_show_prediction.ipynb`           | Python notebook for data prep and modeling  |
| `cleaned_appointments_with_predictions.csv` | Final dataset with model predictions |
| `Appointment_NoShow_Dashboard.pbix`  | Power BI dashboard                          |
| `README.md`                          | Project documentation                       |

---

## ✅ Optimization Recommendations

- Send **SMS reminders** for all appointments
- Avoid scheduling after long waiting periods (>7 days)
- Reschedule or double-confirm high-risk patients (as predicted)
- Monitor low-attendance weekdays and adjust staff accordingly

---

## 📬 Contact

Created by Praveen S 
🔗 LinkedIn: https://www.linkedin.com/in/praveen-s 
📧 Email:praveensp070205@gmail.com

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

