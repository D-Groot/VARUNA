# VARUNA — Prototype Demo

## Demo Objective
Demonstrate how VARUNA processes sample service data, identifies a possible interruption, explains the alert, and prioritizes verification.

## Demo Scenario
A simulated supply zone experiences a sudden reduction in flow. Several synthetic households report no water within a short time window.

## Demonstration Steps
1. Open the village dashboard.
2. Display the incoming sample readings and citizen reports.
3. Inject a labelled simulated outage.
4. Show the anomaly or rule-based trigger.
5. Group related reports into a candidate incident.
6. Display severity, evidence sources, data freshness, and confidence.
7. Show the recommended verification action and priority queue.
8. Mark the incident as verified or unresolved and record the status change.
9. Demonstrate offline queuing and synchronization if implemented.

## Expected Output
- A timestamped incident record.
- An explanation of why it was flagged.
- An explicit distinction between suspected and verified status.
- A prioritized action for the responsible team.
- An audit trail of status changes.

## Evaluation
Record precision, recall, false alerts, duplicate handling, triage time, and synchronization success on a labelled test set.

## Demo Data Warning
All simulated readings and complaints must be labelled as synthetic. They are not evidence of actual water outages or field performance.

## Demo Link
Add the verified public demo URL here after deployment.

## Video Link
Add a recorded demonstration URL here after recording.

## Current Status
Update this section to identify which features are implemented, partially implemented, or planned. Do not claim a feature is working before testing it.
