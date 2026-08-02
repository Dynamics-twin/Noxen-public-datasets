# Noxen Healthcare Engine — Free sample

**100% SYNTHETIC - NO REAL PATIENT DATA USED**

Companion document for the free sample — free to share for evaluation purposes.

<b>⚠️ ILLUSTRATIVE SAMPLE ONLY.</b> This is NOT the actual commercial deliverable — it is a reduced preview meant to show the structure and style of the data before purchase. Volume, granularity and documentation are deliberately limited and do not represent what is delivered in the commercial tiers (100K, 2.5M, 5M, 10M Vital_Signs rows).

## 1. Technical fact sheet

- Edition : SAMPLE (free)
- Tier : `SAMPLE_2000`
- Generation seed : `42`
- Simulated patients : 16
- Simulated time window : 60 days
- Generated on (UTC) : 2026-08-02T09:52:49.096245+00:00
- Number of tables : 17
- Total rows (all tables) : 4 007

## 2. Overview — breakdown by functional domain

| Domain | Tables | Rows |
|---|---|---|
| Reference data | 6 | 74 |
| Patients & encounters | 2 | 36 |
| Clinical events | 7 | 3 878 |
| Billing & outcomes | 2 | 19 |

## 3. Relational schema

| Table | Domain | Rows | Description |
|---|---|---|---|
| `Facility.csv` | Reference data | 1 | Healthcare facilities (reference, capped). |
| `Department.csv` | Reference data | 6 | Clinical departments per facility (reference, capped). |
| `Provider.csv` | Reference data | 36 | Clinicians (reference, capped). |
| `Payer_Plan.csv` | Reference data | 5 | Insurance/payer plans (reference, capped). |
| `Drug_Reference.csv` | Reference data | 15 | Drug reference catalog (reference, capped). |
| `Lab_Test_Reference.csv` | Reference data | 11 | Lab test reference catalog (reference, capped). |
| `Patient.csv` | Patients & encounters | 18 | One record per simulated patient, with age-correlated comorbidities. |
| `Encounter.csv` | Patients & encounters | 18 | Encounters/stays (pivot table linking patients, providers, diagnoses...). |
| `Diagnosis.csv` | Clinical events | 35 | ICD-10 coded diagnoses tied to an encounter. |
| `Procedure.csv` | Clinical events | 17 | Medical procedures (CPT) tied to an encounter. |
| `Vital_Signs.csv` | Clinical events | 3 612 | Vital signs (HR/RR/SBP/DBP/Temp/SpO2) — main volumetric table, equivalent to Sensor_Reading on the aerospace side. |
| `Lab_Result.csv` | Clinical events | 122 | Lab results tied to an encounter. |
| `Medication.csv` | Clinical events | 60 | Medication orders/administrations. |
| `Allergy.csv` | Clinical events | 12 | Patient-reported allergies. |
| `Immunization.csv` | Clinical events | 20 | Patient immunizations. |
| `Billing_Claim.csv` | Billing & outcomes | 18 | Billing claims tied to an encounter. |
| `Death.csv` | Billing & outcomes | 1 | Deaths occurring during an encounter (subset of Encounter). |

> Column-by-column detail (types, primary/foreign keys) is only provided in the commercial version.

## 4. Data quality

Realistic quality defects (missing values, duplicates, coding errors, impossible values, etc.) are injected into this sample. Exact rates and ground-truth label files are only provided in the commercial version.

The commercial version additionally includes: ground-truth label files to distinguish real signal from injected anomaly, detailed column-by-column documentation, and a much larger data volume.

## 5. Use cases

- Training AI/LLM/agent models: readmission prediction, clinical anomaly detection, Text-to-SQL agents.
- Database engineering and data pipeline testing.
- Exploratory analysis, dashboards, product demos.

## 6. Disclaimer

This entire dataset is computer-generated. No data, identifier, or name of any person or organization comes from a real source. Any resemblance to an actual patient, facility, or event is purely coincidental and unintentional.

---

Noxen — 100% SYNTHETIC, NO REAL PATIENT DATA USED.