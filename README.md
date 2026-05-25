-- Wazuh SOC Home Lab

# Overview



#  This project is a beginner-friendly SOC home lab built using Wazuh for security monitoring and threat detection.

The lab was created to simulate real-world SOC activities such as monitoring endpoints, detecting suspicious behavior, and analyzing security events from a Windows machine.



The setup includes a Windows 11 system connected to a Wazuh Manager running on an Ubuntu Server virtual machine.



# What This Lab Demonstrates

File Integrity Monitoring (FIM)

Threat Hunting and Log Analysis

Windows Defender event monitoring

Sysmon event collection

Suspicious PowerShell activity detection

Endpoint visibility using Wazuh

Tools \& Technologies Used

Wazuh

Ubuntu Server VM

Windows 11

Sysmon

Windows Defender

VirtualBox



# Lab Architecture

Windows 11 Host (Wazuh Agent)

         |

         v

Ubuntu Server VM (Wazuh Manager)



# File Integrity Monitoring (FIM)



Configured Wazuh FIM to monitor selected directories and track file activity in real time.



\-Monitored Activities

\-File creation

\-File modification

\-File deletion

\-Checksum/hash changes

\-Detection Results



#  Wazuh successfully detected:



\-Newly added text inside files

\-file modifications

\-Changes in file hashes/checksums

\-Suspicious file activity



This helped demonstrate how SOC analysts can monitor sensitive files for unauthorized changes.



#  Threat Hunting



Used the Wazuh Threat Hunting dashboard to investigate endpoint activity and identify suspicious behavior.



\-Activities Investigated

\-PowerShell execution

\-net.exe discovery commands

\-Suspicious CMD activity

\-Windows event logs

\-Sysmon-generated events



The lab provided hands-on experience with analyzing logs and identifying potentially malicious activity.



#  Malware Detection



Tested malware detection capabilities using the EICAR antivirus test file.



\-Observed Behavior

\-Windows Defender detected the file successfully

\-Wazuh generated security alerts

\-Alerts were visible in the Threat Hunting dashboard

\-Endpoint events were collected and analyzed



## This simulation demonstrated how Wazuh can assist SOC analysts in monitoring malware-related events.

>>Skills Learned

\-SOC monitoring and analysis

\-Threat detection

\-Windows event monitoring

\-Log analysis

\-Endpoint monitoring

\-Basic threat hunting

\-Working with Wazuh dashboards

\-Security event investigation

