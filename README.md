# 🛡 Enterprise Windows Monitoring with Wazuh SIEM

> Enterprise-grade Windows 11 monitoring using **Wazuh SIEM**, **Sysmon**, and **custom detection engineering**.

![Status](https://img.shields.io/badge/Status-In%20Progress-yellow)
![Platform](https://img.shields.io/badge/Platform-Windows%2011-blue)
![SIEM](https://img.shields.io/badge/SIEM-Wazuh-0266C8)
![Sysmon](https://img.shields.io/badge/Sysmon-Enabled-success)
![MITRE](https://img.shields.io/badge/MITRE-ATT%26CK-red)
![License](https://img.shields.io/badge/License-MIT-green)

---

## 📖 Overview

This project demonstrates the implementation of a **Security Information and Event Management (SIEM)** platform focused on monitoring Windows 11 endpoints.

The environment simulates a real **Security Operations Center (SOC)** by combining Windows Event Logs, Sysmon telemetry and custom Wazuh detection rules to identify malicious activities while reducing unnecessary system noise.

The primary monitoring scenarios include:

- 🔌 USB Device Monitoring
- 🖥 Remote Desktop Protocol (RDP)
- 🌐 External Network Connection Monitoring
- ⚙️ Process Monitoring
- 🚨 Threat Detection
- 📊 Custom Security Dashboards
- 🛡 MITRE ATT&CK Mapping

The goal is not only to deploy Wazuh, but to design a realistic detection engineering project following enterprise security monitoring best practices.

---

## 🎯 Project Objectives

- Build a realistic enterprise SIEM laboratory
- Monitor Windows 11 security events
- Detect USB device activity
- Detect successful and failed RDP logins
- Monitor outbound connections to external IP addresses
- Reduce unnecessary Windows event noise
- Create custom Wazuh detection rules
- Build professional security dashboards
- Map detections to the MITRE ATT&CK framework
- Document the entire project from start to finish

---

## ✨ Features

- ✅ Windows 11 Endpoint Monitoring
- ✅ USB Device Detection
- ✅ Remote Desktop Monitoring
- ✅ External IP Monitoring
- ✅ Sysmon Integration
- ✅ Custom Wazuh Rules
- ✅ Noise Reduction
- ✅ Interactive Dashboards
- ✅ MITRE ATT&CK Mapping
- ✅ Threat Detection Engineering
- ✅ Security Event Investigation


---

# 📚 Project Modules

| ID | Module | Technologies | Status |
|:--:|---------|--------------|:------:|
| 01 | [📖 Project Overview](docs/01-project-overview.md) | Documentation | ✅ Completed |
| 02 | [🏗 Architecture](docs/02-architecture.md) | Draw.io | 🟡 In Progress |
| 03 | [⚙ Wazuh Installation](docs/03-wazuh-installation.md) | Ubuntu Server, Wazuh | 🔵 Planned |
| 04 | [🖥 Windows Agent](docs/04-windows-agent.md) | Windows 11, Wazuh Agent | 🔵 Planned |
| 05 | [🛡 Sysmon Configuration](docs/05-sysmon.md) | Sysmon | 🔵 Planned |
| 06 | [🔌 USB Monitoring](docs/06-usb-monitoring.md) | Wazuh, Sysmon | 🔵 Planned |
| 07 | [🖥 RDP Monitoring](docs/07-rdp-monitoring.md) | Windows Event Logs | 🔵 Planned |
| 08 | [🌐 Network Monitoring](docs/08-network-monitoring.md) | Sysmon Network Events | 🔵 Planned |
| 09 | [📜 Custom Detection Rules](docs/09-custom-rules.md) | Wazuh Rules | 🔵 Planned |
| 10 | [🔇 Noise Reduction](docs/10-noise-reduction.md) | Wazuh | 🔵 Planned |
| 11 | [📊 Security Dashboards](docs/11-dashboards.md) | OpenSearch Dashboards | 🔵 Planned |
| 12 | [🧪 Detection Testing](docs/12-testing.md) | Kali Linux, Windows 11 | 🔵 Planned |




## 📑 Table of Contents

- [📖 Overview](#-overview)
- [🎯 Project Objectives](#-project-objectives)
- [✨ Features](#-features)
- [📚 Project Modules](#-project-modules)
- [🏗️ Lab Architecture](#️-lab-architecture)
- [🛠️ Technologies](#️-technologies)
- [📂 Repository Structure](#-repository-structure)
- [🚀 Installation](#-installation)
- [🧪 Testing](#-testing)
- [📊 Dashboards](#-dashboards)
- [🗺️ MITRE ATT&CK Coverage](#️-mitre-attck-coverage)
- [👨‍💻 Author](#-author)

---
---
