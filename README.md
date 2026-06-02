🛡️ Wazuh SOC Home Lab
A beginner-friendly Security Operations Center (SOC) home lab built with Wazuh for security monitoring and threat detection. This lab simulates real-world SOC activities — monitoring endpoints, detecting suspicious behavior, and analyzing security events from a Windows machine.

📋 Table of Contents

Overview
Lab Architecture
Tools & Technologies
Features & Demonstrations

File Integrity Monitoring (FIM)
Threat Hunting & Log Analysis
Malware Detection


Skills Learned


Overview
This lab was built to gain hands-on experience with core SOC workflows, including:

Monitoring endpoints for suspicious activity
Detecting and investigating security events
Analyzing logs from a Windows environment using the Wazuh platform


Lab Architecture
Windows 11 Host (Wazuh Agent)
          |
          ▼
Ubuntu Server VM (Wazuh Manager)
ComponentRoleWindows 11Monitored endpoint running the Wazuh AgentUbuntu Server VMHosts the Wazuh Manager (log aggregation & alerting)VirtualBoxVirtualization platform for the Ubuntu Server VM

Tools & Technologies
ToolPurposeWazuhSIEM / security monitoring platformUbuntu ServerWazuh Manager hostWindows 11Endpoint being monitoredSysmonAdvanced Windows event loggingWindows DefenderAntivirus / malware detectionVirtualBoxVM hypervisor

Features & Demonstrations
File Integrity Monitoring (FIM)
Configured Wazuh FIM to monitor selected directories and track file activity in real time.
Monitored Activities:

File creation, modification, and deletion
Checksum / hash changes

Detection Results:
Wazuh successfully detected:

✅ Newly added text inside files
✅ File modifications
✅ Changes in file hashes/checksums
✅ Suspicious file activity


This demonstrates how SOC analysts can monitor sensitive files and directories for unauthorized changes.


Threat Hunting & Log Analysis
Used the Wazuh Threat Hunting dashboard to investigate endpoint activity and identify suspicious behavior.
Activities Investigated:

PowerShell execution events
net.exe discovery commands
Suspicious CMD activity
Windows event logs
Sysmon-generated events


This provided hands-on experience with log analysis and identifying potentially malicious activity patterns.


Malware Detection
Tested malware detection capabilities using the EICAR antivirus test file.
Observed Behavior:

✅ Windows Defender detected the test file
✅ Wazuh generated corresponding security alerts
✅ Alerts were visible in the Threat Hunting dashboard
✅ Endpoint events were collected and analyzed


This simulation demonstrates how Wazuh supports SOC analysts in monitoring and responding to malware-related events.


Skills Learned

SOC monitoring and analysis
Threat detection and investigation
Windows event monitoring (Event Logs + Sysmon)
Log analysis and correlation
Endpoint visibility and monitoring
Basic threat hunting workflows
Working with Wazuh dashboards
Security event investigation
