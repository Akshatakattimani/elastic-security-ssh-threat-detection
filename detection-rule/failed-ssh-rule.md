# Failed SSH Detection Rule

## Objective

Detect failed SSH authentication attempts collected by Elastic Agent and generate security alerts for investigation.

---

## Detection Strategy

The detection rule monitors SSH authentication failures generated on Linux systems and indexed into Elasticsearch.

These events can indicate:

- Password guessing
- Brute-force attempts
- Invalid user authentication
- Unauthorized access attempts

---

## Data Source

- Elastic Agent
- Linux System Logs
- SSH Authentication Events

---

## Expected Result

When a failed SSH login occurs:

- Event is collected by Elastic Agent.
- Event is indexed into Elasticsearch.
- Detection rule evaluates the event.
- Security alert is generated in Elastic Security.
- Analyst investigates the alert.
