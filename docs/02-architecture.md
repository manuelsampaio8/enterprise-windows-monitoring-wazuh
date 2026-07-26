# 🏗️ Lab Architecture

## Overview

The laboratory was designed to simulate a small enterprise Security Operations Center (SOC) using a centralized SIEM architecture.

The environment consists of three virtual machines running on Oracle VirtualBox:

- Ubuntu Server 24.04 (Wazuh Server)
- Windows 11 Pro (Monitored Endpoint)
- Kali Linux (Attack Workstation)

This architecture allows realistic attack simulations while collecting and analysing security events in real time.

---

# Architecture Diagram

![Lab Architecture](../architecture/architecture.png)

---

# Components

## Ubuntu Server 24.04

The Ubuntu Server hosts the complete Wazuh platform and acts as the central monitoring server.

### Installed Components

- Wazuh Manager
- Wazuh Indexer
- Wazuh Dashboard
- Filebeat
- Wazuh API

Responsibilities:

- Receive events from monitored endpoints
- Correlate security events
- Generate alerts
- Store indexed logs
- Display dashboards

---

## Windows 11 Pro

Windows 11 is the monitored endpoint.

Installed components:

- Wazuh Agent
- Sysmon

Security events collected include:

- Authentication Events
- USB Device Activity
- RDP Sessions
- Process Creation
- Windows Security Logs
- External Network Connections

---

## Kali Linux

Kali Linux is used exclusively for attack simulation.

Typical tools include:

- Nmap
- Hydra
- Metasploit
- Netcat

Attack scenarios include:

- Port Scanning
- Brute Force Attacks
- Reverse Shell Simulation
- External Connections

---

# Event Flow

Security events follow the architecture below:

```
Sysmon
      │
Windows Event Logs
      │
Wazuh Agent
      │
Secure Agent Communication
      │
Wazuh Manager
      │
Wazuh Indexer
      │
Wazuh Dashboard
```

---

# Network Design

All virtual machines run inside Oracle VirtualBox and communicate through the configured virtual network.

Communication flow:

Kali Linux → Windows 11 → Ubuntu Server

---

# Detection Objectives

The project focuses on detecting:

- Failed Authentication
- Successful Logons
- USB Devices
- RDP Sessions
- External Connections
- Process Creation
- PowerShell Activity
- MITRE ATT&CK Techniques
