Project Report: Healthcare Appointment No-Show Prediction
Objective
The objective of this project is to predict whether a patient will miss a scheduled healthcare appointment. By doing so, we aim to optimize appointment scheduling, reduce wasted slots, and improve clinic efficiency.
Tools & Technologies
Python (Pandas, Scikit-learn, Matplotlib)
Power BI (for visual analytics and dashboards)
Dataset: Patient appointment history with features like SMS reminders, age, appointment day, etc.
Dataset Overview
Number of records: ~110,000 appointments
Key Features:
Gender, Age, SMS_received, ScheduledDay, AppointmentDay, Neighbourhood, No-show (target variable)
Data Cleaning and Preprocessing
Removed irrelevant columns like PatientID, AppointmentID.
Converted date columns to datetime format.
Created a new feature: WaitingDays = AppointmentDay - ScheduledDay.
Encoded categorical variables:
Gender (F=0, M=1)
No-show (No=0, Yes=1)
One-hot encoded the Neighbourhood column.
Removed or imputed missing values as needed.
Results and Evaluation
Accuracy: ~74%
Insights:
Younger patients are more likely to miss appointments.
Patients who did not receive an SMS are more likely to be no-shows.
Monday has a higher rate of no-shows compared to other days.
Power BI Dashboard
Exported cleaned data to .csv
Created visualizations for:
No-show distribution by age and gender
SMS reminder effectiveness
No-show trends by weekday
Geographic hotspots of missed appointments
Deliverables
Trained Decision Tree Prediction Model (.pkl file if saved)
Cleaned dataset for Power BI (cleaned_appointments.csv)
Power BI interactive dashboard
This final project report



