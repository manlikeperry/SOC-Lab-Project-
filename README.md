# Home SOC Lab: Attack & Detect

## Overview
This project is a full Security Operations Center (SOC) lab built from scratch to practice real-world attack simulation, detection, and incident response. The lab simulates a small corporate network with a firewall, domain controller, endpoint, and attacker machine.

## Architecture
- **pfSense:** Firewall and router (WAN/LAN, NAT, DHCP, firewall rules).
- **Windows Server 2022:** Domain Controller (Active Directory, DNS, File Server).
- **Windows 10:** Endpoint (joined to domain, monitored by Sysmon).
- **Kali Linux:** Attacker machine (RDP brute-force, scanning).
- **Splunk Enterprise:** SIEM (log ingestion, alerts, dashboards).
- **Sysmon:** Deep endpoint telemetry.
- **Wireshark:** Packet capture and analysis.

## Tools Used
| Tool | Purpose |
|------|---------|
| pfSense | Firewall, NAT, DHCP, LAN rules |
| Splunk Enterprise | SIEM, log analysis, alerts |
| Splunk Universal Forwarder | Log shipping from Windows 10 |
| Sysmon | Process creation and network monitoring |
| Kali Linux | Attack simulation |
| Metasploit / Hydra | Brute-force testing |
| Wireshark | Packet capture and protocol analysis |
| Windows Server 2022 | Active Directory, DNS, File Shares |

## Key Findings
- Detected failed login attempts (EventCode 4625) using Splunk.
- Created a real-time alert for brute-force attacks.
- Used Wireshark to capture and verify ICMP and TCP traffic.
- Blocked a simulated attacker at the pfSense firewall.
- Configured Role-Based Access Control (RBAC) for departmental file shares.

## Lessons Learned
- Gained hands-on experience with SIEM configuration, log analysis, and alert creation.
- Learned how to troubleshoot log forwarding issues (Splunk Universal Forwarder).
- Practiced network segmentation and firewall rule creation.
- Developed a custom Python script for RDP brute-force testing.

## Author
**Perry Wisdom White**  
Cybersecurity Analyst | System Engineer  
[LinkedIn](https://linkedin.com/in/perry-wisdom-white-5ab0a418b)