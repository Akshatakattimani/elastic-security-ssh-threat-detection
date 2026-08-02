# Troubleshooting

## Objective

Document the issues encountered during the Elastic Security home lab setup and the steps taken to resolve them.

---

## Issue 1 – Elastic Agent Enrollment

### Problem

Elastic Agent was unable to enroll successfully with Fleet Server.

### Resolution

- Verified Fleet Server configuration.
- Confirmed enrollment token.
- Reinstalled and re-enrolled Elastic Agent.

---

## Issue 2 – Endpoint Logs Not Visible

### Problem

Authentication events were not appearing in Kibana.

### Resolution

- Verified Elastic Agent status.
- Confirmed System Integration was installed.
- Checked data streams and agent policy.

---

## Issue 3 – Detection Rule Not Triggering

### Problem

Generated SSH authentication events did not initially produce alerts.

### Resolution

- Verified detection rule configuration.
- Confirmed required log fields were available.
- Generated additional SSH authentication events for testing.

---

## Issue 4 – Dashboard Verification

### Problem

Expected security events were missing from dashboard visualizations.

### Resolution

- Adjusted dashboard time range.
- Refreshed Kibana index patterns.
- Verified incoming endpoint telemetry.

---

## Lessons Learned

- Validate Elastic Agent health before troubleshooting detections.
- Confirm data ingestion before investigating dashboards.
- Verify detection rules after each configuration change.
- Generate controlled security events to validate the monitoring pipeline.
