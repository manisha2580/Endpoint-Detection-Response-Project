<img width="505" height="551" alt="image (2)" src="https://github.com/user-attachments/assets/a8ea13d5-0625-4627-af2d-c2d6562d4544" />
<img width="516" height="550" alt="image (3)" src="https://github.com/user-attachments/assets/d4974ecb-baf4-47ba-9e46-eb07d0775f49" />
<img width="1009" height="678" alt="image" src="https://github.com/user-attachments/assets/6aa0e54d-2bc3-48b0-9444-0a6c84a0f2cb" />
<img width="993" height="604" alt="image (1)" src="https://github.com/user-attachments/assets/74eaa6b0-bdd0-49cf-8765-59d27b09d012" />
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
