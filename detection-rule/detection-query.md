# SSH Authentication Detection Query

## Objective

Identify failed SSH authentication attempts collected by Elastic Agent and indexed into Elasticsearch.

---

## Detection Logic

The detection rule analyzes Linux authentication logs for SSH login failures.

The rule focuses on:

- Failed password attempts
- Invalid user logins
- SSH authentication failures
- Unauthorized access attempts

---

## Investigation Workflow

1. Elastic Agent collects Linux system logs.
2. Logs are forwarded to Elasticsearch.
3. Detection rule analyzes incoming events.
4. Matching events generate security alerts.
5. Alerts are investigated in Elastic Security.

---

## Expected Output

Successful detection should display:

- Source host
- Event timestamp
- Authentication failure
- Alert severity
- Detection rule information
