# SOC Home Lab

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

### Key learning:
Splunk CLI uses single-dash flags (e.g. `-user`) unlike standard Linux double-dash (`--user`)

**Status: Complete ✅**
