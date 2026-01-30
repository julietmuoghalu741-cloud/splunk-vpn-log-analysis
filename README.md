# splunk-vpn-log-analysis
This project demonstrates how a SOC analyst ingests and analyzes VPN log data using Splunk SIEM. The objective was to simulate real-world SOC investigation tasks such as monitoring VPN access, analyzing user activity, correlating IP addresses, and reviewing geographic access patterns.
Project Objective

The goal of this project was to ingest VPN log data into Splunk and perform security-focused analysis by examining user logins, source IP addresses, and country-based activity. This simulates how SOC analysts monitor VPN access for suspicious or unusual behavior.
Tools & Environment

Splunk Enterprise (SIEM)

Windows 11

JSON-based VPN log dataset

Splunk Search Processing Language (SPL)


Data Ingestion Process

Uploaded VPN log file using Splunk’s Upload Data feature

Selected _json as the source type to ensure proper field extraction

Created a custom index named VPN_Logs

Verified successful ingestion and data availability


