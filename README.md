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

![IMG_1003 (2)](https://github.com/user-attachments/assets/f6338af6-b7b9-454a-8c22-5b0838076a01)
index=VPN_Logs
Used to determine the total number of VPN events.

![IMG_1004 (2)](https://github.com/user-attachments/assets/2698a5f4-58cf-4a74-ab9c-74eea33b57db)

index=VPN_Logs UserName=Maleena
Analyzed VPN activity associated with a specific user account.

![IMG_1005 (2)](https://github.com/user-attachments/assets/40f49fd1-4e07-45e7-8bbf-7056306e9ef6)

index=VPN_Logs Source_ip=107.xx.xxx.xx
Identified the username associated with a specific IP address.

![IMG_1007 (2)](https://github.com/user-attachments/assets/582ff421-3243-47f3-9c82-4fa9b7ba3692)
index=VPN_Logs Source_Country!=France
Filtered VPN activity originating outside France.

Key Findings

Identified VPN activity linked to specific users

Correlated source IP addresses with user accounts

Observed VPN access from multiple geographic locations

Demonstrated how SIEM tools support SOC investigations


Skills Demonstrated

SIEM log ingestion

Index management in Splunk

SPL-based log analysis

User, IP, and geographic correlation

SOC investigation workflow


Notes

This is a lab-based SOC project created for learning and portfolio development purposes.











Verified successful ingestion and data availability


