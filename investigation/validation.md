# Detection Validation

## Objective

Verify that Elastic Security successfully detects and displays SSH authentication events collected by Elastic Agent.

---

## Validation Process

The generated SSH authentication events were verified using Kibana and Elastic Security.

The investigation confirmed:

- Elastic Agent was actively collecting endpoint logs.
- Authentication events were successfully indexed into Elasticsearch.
- Detection rules analyzed the incoming events.
- Security alerts were generated for investigation.
- Events were available in Kibana for further analysis.

---

## Validation Checklist

- Elastic Agent healthy
- Endpoint logs received
- Detection rule enabled
- Security alerts generated
- Dashboard updated successfully

---

## Result

The detection workflow successfully collected, processed, and displayed SSH authentication events within Elastic Security.
