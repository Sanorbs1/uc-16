# UC-16 Appointment No-Show Reducer

## Objective
Identify appointments at risk of no-show and draft operational reminder messages.

## Business Value
- Prioritize outreach for appointments with higher operational risk.
- Explain why appointments are flagged.
- Prepare reminder message variants for review.
- Provide self-service analytics through Genie.

## Architecture
CSV -> Bronze -> Silver -> Gold -> AI Outreach -> Genie/Dashboard

## Databricks Objects
- Catalog: poc_health_no_show
- Schemas: bronze, silver, gold, ops
- Bronze: appointments_raw
- Silver: appointments_clean, patient_history_features
- Gold: appointment_risk_segments, outreach_message_variants, outreach_tracking_simulated
- Agent: Appointment No-Show Assistant

## Data Sources
Kaggle Medical Appointment No Shows dataset.

## Privacy and Safety
- Patient IDs are pseudonymized.
- No real patient outreach is performed.
- No diagnosis, treatment, or medication advice is generated.
- A/B outcomes are simulated.

## Limitations
- Historical associations do not prove future behavior.
- The risk score is for operational prioritization only.
- Databricks Free Edition is a non-production POC environment.