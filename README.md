# openVAS_Elevatelabs_task3
 🛡️ Cyber Security Internship - Task 3 Objective The objective of this task is to perform a basic vulnerability scan on the local machine using OpenVAS, identify potential security issues, and recommend fixes.

Final Report on Task 3: Basic Vulnerability Scan (OpenVAS on Ubuntu)

Name: DHARANIRAJAN B
Internship: Elevate Lab – Cyber Security Section
Tool Used: OpenVAS (Greenbone Vulnerability Management)
Target: 127.0.0.1 (Localhost)
------------------------------------------------------------
1. Objective
The objective of this task is to perform a basic vulnerability scan on the local machine using OpenVAS, identify potential security issues, and recommend fixes.
------------------------------------------------------------
2. Environment Setup
- Operating System: kali linux (running inside VMware Workstation)
- System Update:
  sudo apt update && sudo apt upgrade -y
------------------------------------------------------------
3. Installation of OpenVAS
- Installed OpenVAS using:
  sudo apt install openvas -y
- Initialized the setup:
  sudo gvm-setup
- Recorded admin username and password for login.
------------------------------------------------------------
4. Starting OpenVAS Services
- Verified setup status:
  sudo gvm-check-setup
- Started services:
  sudo gvm-start
- Accessed web UI at:
  https://127.0.0.1:9392
- Logged in with admin credentials.
------------------------------------------------------------
5. Scan Configuration
- Created a new scan target:
  Configuration → Targets → New Target
  Name: My Localkali
  Hosts: 127.0.0.1
- Created and started a new scan task:
  Scans → Tasks → New Task
  Name: Vulnerability Scan
  Target: My Localkali
  Scan Config: Full and Fast
- Launched the scan.
------------------------------------------------------------
6. Scan Summary
Total Vulnerabilities Found: 9
- Critical: 1
- High: 2
- Medium: 3
- Low: 3
------------------------------------------------------------
7. Critical Vulnerabilities Identified
| CVE ID        | Severity | Vulnerability Description       | Fix or Patch                            |
| ------------- | -------- | ------------------------------- | --------------------------------------- |
| CVE-2021-3156 | Critical | Sudo Heap-Based Buffer Overflow | Update sudo to version 1.9.5p2 or newer |
------------------------------------------------------------
8. Fix Recommendations
- Update outdated software packages to the latest versions.
- Apply all security patches provided by official vendors.
- Disable unused or unnecessary services.
- Restrict open network ports and services.
------------------------------------------------------------
9. Learning Outcome
This task provided hands-on experience in:
- Installing and configuring OpenVAS on Ubuntu.
- Creating and executing vulnerability scans.
- Understanding and interpreting vulnerability reports.
- Identifying and prioritizing security risks using CVSS scores.
- Recommending appropriate security measures.
------------------------------------------------------------
THANK YOU
