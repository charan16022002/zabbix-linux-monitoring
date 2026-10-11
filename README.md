# Zabbix Linux Monitoring Lab

A practical runbook for building a safe lab and monitoring Linux host health with Zabbix.

## Suggested lab workflow

1. Deploy Zabbix Server and a test Linux agent using the official documentation for your chosen version.
2. Register a lab host and link an appropriate Linux template.
3. Confirm latest data for CPU load, memory, filesystem usage, and agent availability.
4. Create or review a trigger for a test threshold.
5. Generate a controlled test condition in a disposable VM and verify the event.
6. Acknowledge, investigate, resolve, and document the event.

## Troubleshooting checklist

- Confirm the agent service is running.
- Check agent and server logs.
- Verify host name and interface configuration.
- Verify network path and configured ports according to your deployment.
- Check item availability, unsupported item errors, trigger expression, and event history.

Use only hosts you are authorized to monitor. Thresholds and ports vary by Zabbix version and deployment. This repository contains the lab guide, not a deployed Zabbix server.
