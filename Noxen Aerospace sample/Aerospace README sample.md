# Noxen Aerospace & MRO Synthetic Dataset — Free sample

**100% SYNTHETIC — NO REAL DATA USED**

Companion document for the free sample — free to share for evaluation purposes.

<b>⚠️ ILLUSTRATIVE SAMPLE ONLY.</b> This is NOT the actual commercial deliverable — it is a reduced preview meant to show the structure and style of the data before purchase. Volume, granularity and documentation are deliberately limited and do not represent what is delivered in the commercial editions (100K / 2.5M / 5M / 10M Sensor_Reading rows).

## 1. Fact sheet

- Edition: SAMPLE (free)
- Number of tables: 18
- Format: CSV (UTF-8, ISO 8601 timestamps)

> Note: the edition name of paid packs (e.g. `WEB_5M`) denotes the target volume of the `Sensor_Reading` table (the largest table), not the total across all tables.

## 2. Overview — breakdown by functional domain

| Domain | Tables |
|---|---|
| Reference data | 7 |
| Operations & fleet | 4 |
| Telemetry & reliability | 4 |
| Maintenance & logistics | 3 |

## 3. Tables included

| Table | Domain | Description |
|---|---|---|
| Airline.csv | Reference data | Synthetic airlines operating the fleet. |
| Aircraft_Model.csv | Reference data | Generic aircraft performance classes. |
| Engine_Model.csv | Reference data | Engine performance classes. |
| Airport.csv | Reference data | Synthetic airports (reserved codes). |
| Fault_Code.csv | Reference data | Fault code reference by ATA chapter. |
| Part.csv | Reference data | Parts catalog. |
| Supplier.csv | Reference data | Synthetic parts suppliers. |
| Aircraft.csv | Operations & fleet | Fleet of aircraft. |
| Technician.csv | Operations & fleet | Maintenance technicians. |
| Flight.csv | Operations & fleet | Scheduled routes. |
| Weather.csv | Operations & fleet | Weather observations per airport. |
| Engine.csv | Telemetry & reliability | Installed engines. |
| Flight_Segment.csv | Telemetry & reliability | Actually operated flights. |
| Sensor_Reading.csv | Telemetry & reliability | Engine/airframe telemetry — main volumetric table. |
| Failure.csv | Telemetry & reliability | Detected failures, with RUL ground truth. |
| Maintenance_Event.csv | Maintenance & logistics | Maintenance actions triggered by a failure. |
| Work_Order.csv | Maintenance & logistics | Detailed work orders. |
| Inventory.csv | Maintenance & logistics | Parts stock movements. |

> Column-by-column detail (types, primary/foreign keys) is only provided in the commercial version.

## 4. Data quality

Realistic quality defects (missing values, sensor drift, stuck-at sensors, impossible values, duplicates, timestamp errors, measurement noise, and more) are injected into this sample, following the same 13 categories used across all Noxen Aerospace editions.

**Included only in the commercial version:** the `Sensor_Reading_quality_labels.csv` ground-truth file (per-reading quality flag) to distinguish real signal from injected anomaly, full column-by-column documentation, and volumes up to 10M+ Sensor_Reading rows.

## 5. Use cases

- Training AI/LLM/agent models: predictive maintenance, anomaly detection, RUL forecasting, Text-to-SQL agents.
- Database engineering and data pipeline testing.
- Exploratory analysis, dashboards, product demos.

## 6. Disclaimer

This entire dataset is computer-generated. No data, identifier, or name of any person or organization comes from a real source. Any resemblance to an actual aircraft, airline, or event is purely coincidental and unintentional.

---

Noxen — 100% SYNTHETIC, NO REAL DATA USED.
