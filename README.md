# Healthconnect-clinic-dataset
The Healthconnect datasets are fictional datasets that shows the records of patients with a No-show appointment. These datasets describe how different factors can affect a patient from not showing up on an appointment .


# HealthConnect – Week 8 Final Data Analytics Package

## Project Overview
This repository contains the final Data Analytics outputs for the HealthConnect appointment/no-show analysis. The work progressed from data preparation and exploratory analysis to deeper segmentation, validation, risk analysis and decision support.

## Final Analytical Scope
The final analysis focuses on:
- Overall appointment outcomes
- No-show and attendance performance
- Previous no-show behaviour
- Booking lead time
- Distance to clinic
- Reminder channels
- Appointment type
- Gender
- Risk-score segmentation
- Appointment day
- Cross-track support for Data Science and Project Management

## Validated Core KPIs
| KPI | Result |
|---|---:|
| Total appointments | 5,000 |
| Total no-shows | 2,423 |
| No-show rate | 48.46% |
| Total attended | 2,314 |
| Attendance rate | 46.28% |
| Total cancelled | 263 |
| Cancellation rate | 5.26% |
| Average waiting time | 24.19 |
| Average booking lead time | 29.64 |
| Average distance | 10.08 |

## Key Findings

### 1. Overall appointment outcome
No-shows represent 48.46% of the 5,000 appointments, while attendance is 46.28% and cancellations are 5.26%.

### 2. Previous no-show behaviour
Appointments involving patients with a previous no-show show a 55.41% no-show rate compared with 43.51% where there was no previous no-show.

### 3. Booking lead time
Observed no-show rate rises across the validated booking-lead groups:
- 0–7 days: 27.81%
- 8–14 days: 33.55%
- 15–30 days: 43.21%
- 31–60 days: 60.49%

### 4. Distance to clinic
The dashboard reports an observed no-show rate of about 68.1% for appointments above 30 km.

### 5. Reminder channels
Observed no-show rates shown on the dashboard are:
- No Reminder: 51.39%
- SMS: 45.75%
- Email: 48.41%
- WhatsApp: 49.77%

These are observational differences and should not be interpreted as proof that a reminder channel causes attendance.

### 6. Appointment type
Observed no-show rates:
- Follow-up: 51.23%
- Diagnostic Test: 49.75%
- Specialist Consultation: 47.44%
- General Consultation: 46.64%

### 7. Risk-score segmentation
The dashboard reports:
- High-risk no-show rate: 69.98%
- Medium-risk no-show rate: 55.70%
- Low-risk no-show rate: 38.55%
- High-risk appointment count: 633
- High-risk no-shows: 443

The high-risk segment is therefore a key candidate for deeper predictive validation.

## Business Recommendations
1. Develop a risk-based appointment monitoring process using validated predictors.
2. Prioritise investigation of previous no-show history, booking lead time and long-distance appointments.
3. Test reminder strategies rather than declaring a channel causally superior from observational data.
4. Consider additional confirmation or rescheduling workflows for long-lead appointments.
5. Investigate operational barriers affecting appointments above 30 km.
6. Use Data Science modelling to test whether the descriptive predictors improve no-show prediction.
7. Use validated findings to support project-management decisions and intervention prioritisation.

## Key Visualisations
The final dashboard should retain:
1. Overall appointment outcome
2. Previous no-show behaviour
3. Booking lead-time no-show rate
4. Distance-group no-show rate
5. Reminder-channel comparison
6. Appointment-type no-show rate
7. Risk-group no-show rate
8. Appointment-day no-show rate
9. Risk segmentation by relevant patient/appointment characteristics

## Analytical Limitations
- The analysis is observational; associations do not establish causality.
- Reminder-channel groups may differ in their underlying patient or appointment characteristics.
- Segment sizes should be checked before interpreting percentages.
- Missing-value treatment can affect derived groups.
- The dataset does not necessarily contain all operational reasons for non-attendance.
- Some dashboard visuals labelled as risk-score analysis appear to show *sums of risk scores* rather than appointment counts. These should be relabelled or replaced with count/rate visuals where appropriate.
- The "Reminder Effectiveness 4.03%" KPI needs a documented numerator/denominator definition before being used as an executive KPI.
- The "Reminder Rate 72.68%" KPI also requires a documented calculation definition.

## Data Science Collaboration
### Data Analytics provides
- Validated KPI definitions
- No-show rates by previous no-show history
- Booking lead-time segmentation
- Distance segmentation
- Reminder-channel comparison
- Appointment-type comparison
- Risk-score segmentation
- Analytical limitations and caveats

### Data Science should test
- Predictive contribution of previous no-show history
- Predictive contribution of booking lead time
- Predictive contribution of distance
- Predictive contribution of reminder variables
- Model performance with and without candidate features
- Feature importance and calibration
- Whether model results confirm or challenge the descriptive findings

## Project Management Contribution
Provide Project Management with:
**Finding → Evidence → Business implication → Recommended action → Validation status**

## Week 8 Finalisation Checklist
- [x] Consolidate validated KPIs
- [x] Refine decision-support visualisations
- [x] Document evidence-based insights
- [x] Document recommendations
- [x] Document limitations
- [x] Prepare cross-track contribution
- [x] Prepare executive summary

## Tools
- Microsoft Excel
- Power Query
- Power BI
- DAX
- GitHub

## Final Executive Statement
The final HealthConnect analysis identifies meaningful variation in appointment outcomes across previous no-show history, booking lead time, distance, reminder channel, appointment type and risk group. The strongest decision-support opportunity is to combine validated descriptive analysis with Data Science modelling so that HealthConnect can distinguish useful predictive indicators from simple associations and translate them into targeted, evidence-based operational actions.

Uploaded and Edited by:
Emmanuel Olisaemeka Echea
