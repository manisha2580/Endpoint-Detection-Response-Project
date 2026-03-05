# Windows 11 SOC & EDR Detection Lab

## Project Goal
To configure a cloud-based/virtualized SIEM environment using **Wazuh** to monitor a Windows 11 endpoint for malicious activity and vulnerabilities.

## Tech Stack
* **Wazuh (SIEM/EDR)** - Log analysis and security monitoring.
* **Windows 11** - Monitored endpoint.
* **PowerShell** - Attack simulation.

## Security Scenarios Simulated
### 1. Privilege Escalation (Critical Alert)
* **Action:** Created a new user and added them to the local 'Administrators' group via PowerShell.
* **Detection:** Triggered **Rule 60154 (Level 12)**.
* **Analysis:** Mapped to MITRE ATT&CK **T1078 (Valid Accounts)** and **T1548 (Abuse Elevation Control Mechanism)**.

### 2. Vulnerability Management
* **Action:** Automated baseline scanning for unpatched software and OS vulnerabilities.
* **Detection:** Identified critical **CVEs** (Common Vulnerabilities and Exposures) from 2022.
