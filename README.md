Analyzing Raw Firewall Logs with Splunk

Overview
Basic analysis of simulated firewall logs using Splunk to identify potential anomalies and suspicious activity.

Tools

Splunk

Data Source

https://github.com/splunk/attack_data

What I Did

Ingested raw firewall logs into Splunk
Parsed comma-separated data into usable fields
Searched for large data transfers and unusual patterns
Reviewed firewall alerts and flagged activity

Key Observations

One large outbound transfer (~1.2MB) stood out as an outlier
Multiple DNS requests to a domain controller in a short timeframe
Repeated VPN alerts from a single host
Database system making DNS requests flagged as alerts

Conclusion
No confirmed malicious activity, but several anomalies were identified that would require deeper investigation with additional logs (e.g., DNS, VPN, packet capture).# firewall_log_analysis_with_spunk
Using Splunk to parse and analyze a raw firewall log.
