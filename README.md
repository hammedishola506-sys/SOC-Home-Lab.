<img width="1010" height="584" alt="image" src="https://github.com/user-attachments/assets/b7213418-9821-48d2-8e03-da3858ba5bdc" /># SOC Home Lab

## Overview
A hands-on Security Operations Center (SOC) home lab built to develop practical cybersecurity skills in network monitoring, threat detection, and incident response.

## Lab Environment
- **Host OS:** Windows 11
- **Virtualization:** VMware Workstation Pro 17
- **Network VM:** mydfir-netlab (imported OVF)

## Virtual Machines
| VM | OS | Purpose |
|----|----|---------|
| Ubuntu Server | Ubuntu 22.04 LTS | Zeek & Suricata IDS/IPS |
| Windows 10 | Windows 10 x64 | Endpoint monitoring |

## Tools Installed
### Network Detection
- **Zeek** - Network traffic analyzer with JA3 & JA4 fingerprinting
- **Suricata** - IDS/IPS with Sliver C2 detection rules
- **Wireshark** - Packet capture and analysis

## Skills Demonstrated
- VM setup and network configuration
- Linux server administration
- IDS/IPS deployment and configuration
- Network traffic analysis
- SSH remote administration

## Course
Following the **mydfir SOC Analyst** course﻿# SOC Home Lab
## ✅ Phase 2 – Splunk Enterprise Installation

### What was done:
- Downloaded and installed Splunk Enterprise (60-day trial) on Ubuntu VM
- Started Splunk and configured it to auto-run on boot:
```bash
  sudo ./splunk enable boot-start -user splunk
```
- Troubleshot VM networking: switched VMware adapter from **NAT → Bridged** to allow host machine access
- Confirmed Splunk web UI accessible at `http://<VM-IP>:8000`
## ✅ Phase 3 – Malware Analysis Environment Setup

### What was done:
- Imported REMnux VM (Ubuntu-based Linux malware analysis toolkit)
- Installed FlareVM on Windows 10 VM (Mandiant's malware analysis toolkit)
- Configured VMware networking: NAT → Bridged for host access
- Completed Day 21 Lab Environment Validation checkpoint

### Lab Environment Summary:
| VM | OS | Purpose |
|----|----|---------|
| Ubuntu 64-bit (2) | Ubuntu 22.04 | Splunk SIEM |
| Windows 10 x64 (2) | Windows 10 | FlareVM / Endpoint |
| Remnux2 | Ubuntu (Noble) | Malware Analysis |
| mydfir-netlab | Linux | Network VM |

### Key learning:
Never disable antivirus on host machine — only inside the VM!

**Status: Complete ✅**
