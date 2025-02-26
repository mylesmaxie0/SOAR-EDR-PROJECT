#  SOAR & EDR Threat Detection with LimaCharlie (In Progress)

📝 Summary:
This project showcases the implementation of LimaCharlie as an EDR solution for detecting and responding to security incidents. It focuses on automated detection and response integration within a SOAR framework.


🔍 Key Implementation Steps:
Deploying LimaCharlie Agents on Windows endpoints for real-time security monitoring.
Configuring custom detection rules to identify threats such as:
- Unauthorized command execution (e.g, suspicious PowerShell and Command Line use).
- Privilege escalation attempts (e.g., running processes as SYSTEM).

Defining automated response actions, including:
- 	Isolating compromised hosts to prevent lateral movement.
- Killing suspicious processes before they execute malicious payloads.

  
