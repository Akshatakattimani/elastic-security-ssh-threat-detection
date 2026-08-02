# Attack Simulation

## Objective

Generate SSH authentication events to verify that Elastic Security successfully collects, detects, and analyzes endpoint activity.

---

## Test Scenario

A Windows virtual machine initiated an SSH connection to the Kali Linux virtual machine.

The SSH login intentionally used an incorrect password to generate authentication failure events.

---

## Environment

- Source: Windows Virtual Machine
- Destination: Kali Linux Virtual Machine
- Service: OpenSSH
- Monitoring: Elastic Agent

---

## Expected Outcome

The failed authentication event should:

- Be collected by Elastic Agent.
- Be indexed into Elasticsearch.
- Trigger the detection rule.
- Generate an alert in Elastic Security.
- Be available for investigation in Kibana.
