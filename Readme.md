# HealthConnect – Advanced Analytics & Decision Support

## Week 6 Data Analytics Project

### Project Overview

This project focuses on analysing HealthConnect appointment data to identify factors associated with patient no-shows and develop evidence-based recommendations to support healthcare appointment management.

Week 6 builds on the data preparation and exploratory analysis completed in Week 5. Instead of repeating the previous EDA, the project focuses on deeper analysis, validation of findings, risk segmentation, decision support and cross-track collaboration with the Data Science team.

---

## Project Objectives

The main objectives of the Week 6 analysis were to:

- Validate key findings and KPIs from Week 5.
- Investigate factors associated with appointment no-shows.
- Examine previous no-show behaviour.
- Evaluate reminder channel effectiveness.
- Investigate the relationship between distance to clinic and appointment attendance.
- Examine appointment-type differences.
- Review gender differences in appointment outcomes.
- Investigate additional factors such as booking lead time.
- Develop a risk-segmentation approach.
- Translate analytical findings into actionable business recommendations.
- Provide relevant variables and analytical questions to the Data Science track for predictive modelling.

---

## Dataset

The HealthConnect dataset contains appointment-level information including:

- Appointment ID
- Patient ID
- Gender
- Age
- Age Group
- Appointment Type
- Booking Date
- Appointment Date
- Appointment Day
- Appointment Time
- Booking Lead Days
- Previous Appointments
- Previous No-Shows
- Reminder Sent
- Reminder Channel
- Distance to Clinic
- Waiting Time
- Appointment Outcome

---

## Week 5 Baseline KPIs

The Week 5 analysis established the following baseline metrics:

| KPI | Result |
|---|---:|
| Total Appointments | 5,000 |
| Total Patients | 1,696 |
| No-Show Rate | 48.46% |
| Attendance Rate | 46.28% |
| Cancellation Rate | 5.26% |
| Average Waiting Time | 24.19 minutes |

These KPIs were used as the baseline for Week 6 validation and deeper analysis.

---

## Week 6 Advanced Analysis

### 1. Previous No-Show Behaviour

Patients with previous no-show behaviour recorded a higher current no-show rate than patients without previous no-shows.

- Previous no-show: 55.41%
- No previous no-show: 43.51%

This indicates that previous attendance behaviour may be useful for identifying appointments requiring additional engagement.

### 2. Reminder Channel Effectiveness

Reminder performance was compared across:

- SMS
- WhatsApp
- Email
- No Reminder

SMS recorded the lowest observed no-show rate among the reminder channels analysed.

The analysis indicates an association between reminder receipt/channel and appointment outcomes. However, the results should not be interpreted as proof of causation because the data is observational.

### 3. Appointment Type

No-show rates were compared across appointment types.

Follow-up appointments recorded the highest observed no-show rate among the appointment types analysed.

This suggests that follow-up appointments may require additional patient engagement and confirmation strategies.

### 4. Distance to Clinic

Distance was analysed using grouped distance categories.

Patients located more than 30 km from the clinic recorded the highest observed no-show rate, approximately 68.1%.

This suggests that geographic accessibility may be an important factor affecting appointment attendance.

### 5. Gender

No-show behaviour was compared across gender groups.

The observed differences between gender groups were relatively small compared with behavioural and accessibility-related factors.

Gender was therefore treated as a monitoring variable rather than a primary intervention variable.

### 6. Booking Lead Time

Booking lead time was introduced as an additional Week 6 investigation.

The analysis examined whether appointments booked further in advance were more likely to result in no-shows.

This variable was selected for deeper investigation because longer periods between booking and appointment may create greater opportunities for missed appointments or changes in patient circumstances.

---

## Risk Segmentation

A preliminary risk-segmentation framework was developed to identify appointments that may require additional engagement.

Potential risk factors included:

- Previous no-show behaviour
- Long booking lead time
- Greater distance from clinic
- Absence of a reminder
- Follow-up appointment type

The risk segmentation is an analytical decision-support tool and should not be considered a validated predictive model.

Formal predictive validation is recommended through the Data Science track.

---

## Key Findings

1. No-shows represent a major operational challenge, accounting for approximately 48.46% of appointments.
2. Patients with previous no-shows have a substantially higher current no-show rate.
3. Reminder channels show differences in observed no-show rates, with SMS performing best among the channels analysed.
4. Patients located more than 30 km from the clinic have the highest observed no-show rate.
5. Follow-up appointments have the highest observed no-show rate among appointment types.
6. Gender shows relatively limited differences and appears less important than behavioural and accessibility-related factors.

---

## Business Recommendations

### 1. Develop targeted high-risk appointment identification

Use historical appointment behaviour and relevant operational factors to identify appointments that may require additional engagement.

### 2. Strengthen reminder strategies

Prioritise testing of SMS reminders and investigate the effectiveness of different reminder timings.

### 3. Target patients with previous no-shows

Patients with previous no-show behaviour should receive stronger confirmation and engagement processes.

### 4. Review long-lead appointments

Appointments booked significantly in advance should receive additional confirmation or reminder interventions.

### 5. Improve access for distant patients

Consider telemedicine, alternative clinic locations or flexible appointment options for patients living far from the clinic.

### 6. Avoid unnecessary demographic targeting

Gender should not be treated as a primary intervention variable unless further analysis provides stronger evidence.

---

## Data Science Cross-Track Collaboration

The Data Analytics track will provide the Data Science track with:

- Cleaned HealthConnect data
- `is_no_show` target variable
- Appointment-level predictor variables
- Previous no-show indicators
- Booking lead time
- Distance to clinic
- Reminder information
- Appointment type
- Demographic variables

### Suggested Data Science Tasks

The Data Science track is expected to investigate:

1. Logistic regression for no-show prediction.
2. Feature importance.
3. No-show probability for each appointment.
4. Model performance using appropriate evaluation metrics.
5. Confusion matrix.
6. Precision, recall and F1-score.
7. ROC-AUC.
8. Cross-validation or appropriate train/test validation.
9. Important interaction effects between risk factors.

### Expected Contribution

The Data Science results should help validate whether the factors identified through EDA and advanced analytics are reliable predictors of no-show behaviour.

The results can also be used to refine the proposed HealthConnect risk-segmentation approach.

---

## Dashboard

The Week 6 Power BI dashboard contains:

### Executive Dashboard

- Total Appointments
- Total Patients
- No-Show Rate
- Attendance Rate
- Average Waiting Time
- Cancellation Rate
- Overall Appointment Outcome
- Appointment Type
- Previous No-Show Behaviour
- Gender
- Reminder Channel Effectiveness
- Distance to Clinic

### No-Show Risk & Decision Support

The second dashboard page focuses on advanced analysis and decision support, including relationships between risk factors, appointment outcomes and no-show behaviour.

---

## Tools Used

- Microsoft Excel
- Power Query
- Power BI
- DAX
- GitHub

---

## Data Limitations

The analysis has several limitations:

- The dataset is observational.
- Associations do not necessarily imply causation.
- Reminder effectiveness may be affected by selection bias.
- Some potentially important factors may not be captured in the dataset.
- The proposed risk score is not a clinically validated prediction model.
- Predictive modelling should be validated on unseen data before operational deployment.

---

## Week 6 Outcome

The Week 6 project progressed from descriptive analysis toward advanced analytics and decision support.

The major outcome was the identification and prioritisation of factors associated with appointment no-shows, validation of Week 5 findings, development of preliminary risk segmentation, and translation of analytical evidence into practical HealthConnect recommendations.

Uploaded and Edited by:
Emmanuel Olisaemeka Echea
