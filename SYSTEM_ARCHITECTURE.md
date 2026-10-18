# VARUNA — System Architecture

## 1. Architecture

Data sources → Ingestion and validation → Incident analysis → Risk prioritization → Dashboard and action tracking.

## 2. Components

### Data ingestion
Accept sample sensor readings, citizen reports, and maintenance records. Validate timestamps, measurement units, and identifiers.

### Storage
Use SQLite for a lightweight prototype. Store incident records, source references, verification status, and audit events.

### Analytics
Start with transparent threshold rules and a baseline detector. Add time-series anomaly detection only when enough suitable data is available. Use clustering to group reports by time, location, and category.

### Incident prioritization
Use a documented scoring rule incorporating severity, duration, affected-household estimates, evidence strength, and data freshness. Calibrate weights through testing rather than treating them as validated probabilities.

### Dashboard
Show service status, incident details, evidence, confidence, unresolved reports, and maintenance actions. Missing data must not be interpreted as proof of normal service.

### Offline workflow
Queue reports locally and synchronize after reconnection. Test duplicate prevention and conflict handling.

### Integration adapter
Prepare a mapping layer for authorized IMIS/Sujal Gaon identifiers. Live integration requires approved access, compatible schemas, and authentication.

## 3. Suggested Stack
Python, Pandas, Streamlit or React, FastAPI if an API is needed, SQLite, and scikit-learn if a trained model is justified.

## 4. Security
Use role-based access where applicable, avoid unnecessary personal data, protect credentials, and log important status changes.

## 5. Limitations
The initial demo is not a certified water-quality monitoring system. It cannot establish potability without suitable validated measurements and procedures.
