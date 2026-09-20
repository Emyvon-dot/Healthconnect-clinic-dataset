# Healthconnect-clinic-dataset
The Healthconnect datasets are fictional datasets that shows the records of patients with a No-show appointment. These datasets describe how different factors can affect a patient from not showing up on an appointment .

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


# HealthConnect – Data Analytics

## Week 7: Analytics Testing, Validation & Refinement

### Project Overview

The HealthConnect Data Analytics project analyses appointment data to understand appointment attendance and no-show behaviour and to develop evidence-based decision support.

Week 7 focused on validating the findings and KPIs developed during Week 6 using independent Excel calculations, pivot-table analysis and Power BI validation.

The analysis concentrated on:

- Appointment outcomes
- No-show behaviour
- Previous no-show history
- Reminder-channel effectiveness
- Distance to clinic
- Booking lead time
- Appointment type
- Risk segmentation

---

## Dataset Overview

The dataset contains 5,000 appointments.

### Validated appointment outcomes

| Outcome | Count | Rate |
|---|---:|---:|
| Attended | 2,314 | 46.28% |
| No-show | 2,423 | 48.46% |
| Cancelled | 263 | 5.26% |
| Total | 5,000 | 100% |

---

## Week 7 Validation

The Week 7 validation process compared dashboard outputs with independent Excel calculations and pivot-table results.

### KPI validation included:

- Total appointments
- Total attended
- Total no-shows
- Total cancellations
- No-show rate
- Attendance rate
- Cancellation rate
- Average waiting time
- Average booking lead time

### Important validation correction

An initial Excel validation cell labelled "No-Show Rate" displayed 5.26%.

This value represents the cancellation rate.

The validated no-show rate is:

**2,423 / 5,000 = 48.46%**

The KPI label/value should therefore be corrected before final submission.

---

## Validated Findings

### 1. Previous No-Show Behaviour

| Previous No-Shows | No-Show Rate |
|---:|---:|
| 0 | 43.51% |
| 1 | 53.49% |
| 2 | 59.36% |
| 3 | 67.95% |
| 4 | 66.67% |
| 5 | 100.00% |

The analysis shows increasing observed no-show rates as previous no-show history increases, particularly from 0 to 3 previous no-shows.

Small subgroup sizes should be considered when interpreting the highest values.

---

### 2. Distance to Clinic

The highest observed no-show rate occurred among appointments involving patients located more than 30 km from the clinic.

**Above 30 km: 68.06%**

Distance is therefore an important candidate variable for further predictive analysis.

---

### 3. Booking Lead Time

| Booking Lead Group | No-Show Rate |
|---|---:|
| 0–7 days | 27.81% |
| 8–14 days | 33.55% |
| 15–30 days | 43.21% |
| 31–60 days | 60.49% |

Longer booking lead time is associated with substantially higher observed no-show rates.

---

### 4. Reminder Channel

| Reminder Channel | No-Show Rate |
|---|---:|
| SMS | 45.75% |
| Email | 48.41% |
| WhatsApp | 49.77% |
| No Reminder | 51.39% |

SMS recorded the lowest observed no-show rate among the reminder categories analysed.

The analysis is observational and does not establish that reminder channel causes differences in attendance.

---

### 5. Appointment Type

| Appointment Type | No-Show Rate |
|---|---:|
| Follow-up | 51.23% |
| Specialist Consultation | 47.44% |
| General Consultation | 46.64% |

Follow-up appointments recorded the highest observed no-show rate.

---

## Updated Recommendations

1. Correct and standardise KPI definitions across Excel and Power BI.
2. Investigate targeted engagement for patients with previous no-show history.
3. Investigate additional confirmation for appointments booked significantly in advance.
4. Explore accessibility solutions for patients located more than 30 km from the clinic.
5. Continue evaluating reminder channels by patient and appointment segment.
6. Use predictive modelling before deploying the preliminary risk segmentation.
7. Avoid treating demographic variables as primary intervention variables without sufficient evidence.

---

## Data Science Cross-Track Collaboration

The Data Analytics track will provide validated analytical findings and candidate features to the Data Science track.

### Candidate modelling features

- Previous no-shows
- Booking lead days
- Distance to clinic
- Reminder received
- Reminder channel
- Appointment type
- Age
- Gender
- Waiting time
- Previous appointments

### Target variable

`is_no_show`

### Data Science validation questions

- Which variables are strongest predictors?
- Does previous no-show history remain predictive?
- Does distance remain predictive?
- Does booking lead time remain predictive?
- Does reminder channel add predictive value?
- Do interaction effects improve the model?
- Does the predictive model support the proposed risk segmentation?

### Expected outputs

- Predictive model
- Feature importance
- No-show probability
- Confusion matrix
- Precision
- Recall
- F1-score
- ROC-AUC
- Validation results
- Model limitations

---

## Week 8 Focus

Week 8 will focus on final integration and decision support.

Planned activities include:

- Correcting validated KPI issues
- Integrating Data Science findings
- Refining the risk-segmentation approach
- Updating Power BI visualisations
- Presenting validated insights
- Translating findings into evidence-based recommendations
- Documenting limitations
- Preparing the final project presentation

---

## Limitations

- The data is observational.
- Associations do not necessarily imply causation.
- Some subgroups may have small sample sizes.
- Reminder-channel analysis may be affected by selection effects.
- Missing waiting-time and distance values were imputed.
- Risk segmentation requires predictive validation.
- The dataset may not contain all factors affecting appointment attendance.

---

## Tools

- Microsoft Excel
- Power Query
- Power BI
- DAX
- GitHub

---

## Project Outcome

Week 7 progressed the HealthConnect project from descriptive and exploratory analysis toward validated analytics and decision support.

The validation confirmed several important patterns involving previous no-show behaviour, booking lead time, distance to clinic, reminder channels and appointment type, while also identifying a KPI labelling error requiring correction.

The validated findings will be used as inputs for Data Science predictive modelling and final Week 8 integration.
