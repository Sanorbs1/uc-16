| Table                           | Column             | Type    | Description                                 |
| ------------------------------- | ------------------ | ------- | ------------------------------------------- |
| silver.appointments_clean       | appointment_id     | string  | Unique appointment identifier               |
| silver.appointments_clean       | patient_pseudo_id  | string  | SHA-256 pseudonymized patient ID            |
| silver.appointments_clean       | lead_time_days     | int     | Days between scheduling and appointment     |
| silver.appointments_clean       | no_show_flag       | boolean | True if patient did not attend              |
| silver.patient_history_features | prior_appointments | int     | Historical appointments before current date |
| silver.patient_history_features | prior_no_show_rate | double  | Historical no-show proportion               |
| gold.appointment_risk_segments  | risk_score         | int     | Transparent operational risk score          |
| gold.appointment_risk_segments  | risk_segment       | string  | HIGH, MEDIUM_HIGH, MEDIUM, LOW              |
| gold.appointment_risk_segments  | risk_reason        | string  | Human-readable explanation                  |
| gold.outreach_message_variants  | message_text       | string  | AI-drafted reminder message                 |