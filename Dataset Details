# VARUNA — Dataset Details

## 1. Data Sources

| Source | Intended use | Access condition |
|---|---|---|
| Jal Jeevan Mission portal — https://jaljeevanmission.gov.in/ | Programme documents and public reports | Publicly accessible content; check reuse terms |
| JJM IMIS reports — https://ejalshakti.gov.in/IMISReports/MIS.html | Available scheme and service reporting | Use accessible public reports; do not assume API or bulk access |
| JJM WQMIS — https://ejalshakti.gov.in/WQMIS/ | Water-quality monitoring context | Check access and download permissions |
| data.gov.in — https://data.gov.in/ | Search for relevant open datasets | Verify dataset licence, fields, and coverage individually |

## 2. Prototype Data
If real household-level data is unavailable, generate synthetic records for testing. Label all generated data as SYNTHETIC. Do not present it as government or field data.

## 3. Suggested Fields
- timestamp
- village_id / gram_panchayat_id
- household_id (synthetic or pseudonymized)
- sensor_id and measurement_type
- flow_rate and pressure, where available
- measurement_unit
- quality_measurement and sensor_source, where available
- complaint_category and complaint_timestamp
- incident_status
- verification_status
- maintenance_action and closure_timestamp

Only include fields supported by the actual dataset or simulator.

## 4. Preprocessing
- Normalize timestamps and units.
- Validate missing and out-of-range values.
- Remove duplicate test records.
- Keep source and data freshness metadata.
- Separate training, validation, and test periods for time-series evaluation.

## 5. Privacy and Security
Do not publish names, phone numbers, exact household locations, credentials, or restricted government data. Use synthetic identifiers for the public demo.

## 6. Data Limitations
Public scheme-level information may not contain real-time household-level flow or pressure. Confirm actual field availability before claiming household-level predictive accuracy.

## 7. Reproducibility
Document the dataset version, retrieval date, licence, schema, preprocessing steps, and random seed for synthetic data.
