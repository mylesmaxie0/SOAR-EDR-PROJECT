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

#
SOAR (Security Orchestration, Automation, and Response)

- Orchestration: Integrates security tools (SIEM, firewalls, Anti-virus) for seamless communication.
- Automation: Reduces security analyst workload by handling repetitive tasks.
- Response: Uses playbooks for faster, consistent incident handling.

EDR (Endpoint Detection and Response)

- Real-Time Monitoring: Detects suspicious endpoint activities (malware, unauthorized access).
- Threat Detection: Uses machine learning & behavioral analysis to spot known/unknown threats.
- Incident Investigation: Provides detailed logs for forensic analysis.
- Automated Responses: Can isolate compromised endpoints and kill malicious processes.
#

### Playbook Workflow

Playbook Objective: 

- Send a Slack Message
- Send an Email - The email will contain Time, Endpoint Name, Source IP, Process, Command Line, File Path, Sensor ID
- Generate a user prompt - Isolate the endpoint. (Yes/No)
- If YES - Lima Charlie will isolate the endpoint.
- If No - Lima Charlie will not isolate.

![image](https://github.com/user-attachments/assets/759b58dd-938a-4d70-9c64-c982e06036b7)
