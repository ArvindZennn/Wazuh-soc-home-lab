# 🛡️ Wazuh SOC Home Lab

> A hands-on Security Operations Center (SOC) home lab focused on SIEM deployment, endpoint monitoring, attack simulation, security detection, log analysis, and incident response.

## 📌 Project Overview

This project documents the development of a practical SOC home lab using **Wazuh**, Windows Server, Active Directory, Ubuntu, and security testing techniques.

The lab was designed to simulate a simplified SOC environment where security events are generated, collected, detected, investigated, and documented.

### SOC Investigation Workflow

```text
┌─────────────────────┐
│   Lab Environment   │
└──────────┬──────────┘
           │
           ▼
┌─────────────────────┐
│   Endpoint / Server │
└──────────┬──────────┘
           │
           ▼
┌─────────────────────┐
│   Wazuh Agent       │
└──────────┬──────────┘
           │
           ▼
┌─────────────────────┐
│   Wazuh SIEM        │
│   Detection Engine  │
└──────────┬──────────┘
           │
           ▼
┌─────────────────────┐
│ Security Alert      │
└──────────┬──────────┘
           │
           ▼
┌─────────────────────┐
│ SOC Investigation   │
└──────────┬──────────┘
           │
           ▼
┌─────────────────────┐
│ Incident Report     │
└─────────────────────┘
```

---

## 🎯 Objectives

The main objectives of this home lab are:

* Build a practical SOC environment
* Deploy and configure Wazuh SIEM
* Monitor Linux endpoints
* Understand security event collection
* Simulate controlled attacks in an isolated environment
* Detect suspicious authentication activity
* Analyze security alerts and logs
* Investigate security incidents
* Document findings using an incident-response workflow

---

## 🏗️ Lab Environment

| Component      | Purpose                                         |
| -------------- | ----------------------------------------------- |
| Windows Server | Active Directory / Windows lab environment      |
| Ubuntu         | Endpoint and security testing                   |
| Wazuh Manager  | SIEM and security monitoring                    |
| Wazuh Agent    | Endpoint telemetry collection                   |
| SSH            | Attack simulation and authentication monitoring |
| VirtualBox     | Virtual lab infrastructure                      |
| Obsidian       | Technical documentation                         |
| GitHub         | Project documentation and portfolio             |

---

## 🔐 Projects & Investigations

### 01 — Active Directory Home Lab

Built a Windows Server Active Directory environment to understand enterprise identity and endpoint administration.

**Topics covered:**

* Windows Server
* Active Directory Domain Services
* Domain Controller
* DNS
* User management
* Domain joining
* Group Policy
* Windows endpoint administration

📂 [View Active Directory Lab](./01-active-directory/)

---

### 02 — Wazuh SOC Lab

Deployed Wazuh to create a centralized security monitoring environment.

**Topics covered:**

* Wazuh Manager
* Wazuh Agent
* Endpoint monitoring
* Security event collection
* Alert generation
* Log analysis
* SOC monitoring

📂 [View Wazuh SOC Lab](./02-wazuh-soc-lab/)

---

### 03 — SSH Brute-Force Attack Simulation

Performed a controlled SSH authentication attack against a lab endpoint to generate security events.

**Purpose:**

Understand how suspicious authentication activity appears in endpoint logs and how a SIEM can detect the activity.

📂 [View Attack Simulation](./02-wazuh-soc-lab/04-attack-simulation/)

---

### 04 — Wazuh Detection & Investigation

Analyzed the generated security events using Wazuh and investigated the resulting alerts.

**Investigation process:**

```text
Attack Simulation
       ↓
Authentication Events
       ↓
Wazuh Agent
       ↓
Wazuh Manager
       ↓
Security Alert
       ↓
Alert Analysis
       ↓
Investigation
       ↓
Findings
```

📂 [View Detection Analysis](./02-wazuh-soc-lab/05-detection-analysis/)

---

### 05 — Incident Response Report

Documented the SSH brute-force activity as a security incident.

The report covers:

* Incident overview
* Attack activity
* Evidence
* Detection
* Investigation
* Findings
* Response
* Recommendations
* Lessons learned

📂 [View Incident Report](./03-incident-response/)

---

## 🧰 Tools & Technologies

**Operating Systems**

* Windows Server
* Windows 11
* Ubuntu Linux

**Security**

* Wazuh
* SIEM
* Security monitoring
* Log analysis
* Incident response

**Networking**

* TCP/IP
* DNS
* SSH
* Network troubleshooting

**Infrastructure**

* VirtualBox

**Documentation**

* Obsidian
* GitHub
* Markdown

---

## 📊 Skills Demonstrated

Through this project, I have practiced:

* SIEM deployment
* Endpoint monitoring
* Log analysis
* Security alert investigation
* Linux administration
* Windows administration
* Active Directory
* Authentication monitoring
* Attack simulation
* Detection analysis
* Incident documentation
* Basic incident response

---

## 🔎 Investigation Methodology

The lab follows a simplified SOC investigation lifecycle:

```text
01. Prepare
      ↓
02. Generate Security Event
      ↓
03. Collect Telemetry
      ↓
04. Detect Alert
      ↓
05. Investigate
      ↓
06. Identify Findings
      ↓
07. Respond
      ↓
08. Document
      ↓
09. Improve Detection
```

---

## 📚 Key Learning Outcomes

This project helped me understand how a SOC environment connects:

**Endpoints → Agents → SIEM → Alerts → Investigation → Incident Response**

It also provided hands-on experience with security monitoring rather than relying only on theoretical cybersecurity concepts.

---

## 🚀 Future Improvements

Planned improvements include:

* Windows endpoint monitoring with Wazuh
* File Integrity Monitoring
* Windows authentication attack detection
* PowerShell activity monitoring
* Malware detection exercises
* Network traffic analysis
* MITRE ATT&CK mapping
* Custom Wazuh detection rules
* Automated response
* Additional incident-response scenarios

---

## 📁 Repository Structure

```text
Wazuh-soc-home-lab/
│
├── README.md
│
├── 01-active-directory/
│
├── 02-wazuh-soc-lab/
│   ├── 01-deployment/
│   ├── 02-agent-setup/
│   ├── 03-verification/
│   ├── 04-attack-simulation/
│   └── 05-detection-analysis/
│
├── 03-incident-response/
│
├── evidence/
│   ├── active-directory/
│   ├── wazuh/
│   ├── attack-simulation/
│   └── detection/
│
└── docs/
```

---

## ⚠️ Disclaimer

All attack simulations and security testing activities documented in this repository were performed in an isolated, authorized home-lab environment for educational and defensive security purposes.

---

## 👨‍💻 Author

**Aravindan K**

Aspiring SOC Analyst | IT Support | Cybersecurity Enthusiast

> **Learn → Build → Detect → Investigate → Document**
