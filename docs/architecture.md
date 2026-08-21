# SOC Home Lab Architecture

## Architecture Overview

The SOC home lab was built using virtual machines to create an isolated environment for security monitoring, controlled attack simulation, detection, investigation, and incident response.

## Lab Architecture

```text
                    SOC HOME LAB
                         |
          +--------------+--------------+
          |                             |
          ↓                             ↓
   Windows Server                  Ubuntu Endpoint
   Active Directory                Wazuh Agent
          |                             |
          ↓                             ↓
   Windows Client              Security Telemetry
                                        |
                                        ↓
                                Wazuh Manager
                                        |
                                        ↓
                                Security Events
                                        |
                                        ↓
                                   Detection
                                        |
                                        ↓
                                     Alert
                                        |
                                        ↓
                                SOC Investigation
                                        |
                                        ↓
                                Incident Response


Security Monitoring Flow
Endpoint
   ↓
Security Telemetry
   ↓
Wazuh Agent
   ↓
Wazuh Manager
   ↓
Detection Rules
   ↓
Security Alert
   ↓
SOC Investigation
   ↓
Incident Response


Lab Components
Component	Purpose
Windows Server	Active Directory infrastructure
Windows Client	Domain-joined endpoint
Ubuntu	Linux monitored endpoint
Wazuh Agent	Endpoint telemetry collection
Wazuh Manager	Centralized security monitoring
VirtualBox	Virtualization platform
Project Objective

The objective of this lab is to build a practical SOC environment where security events can be generated, collected, detected, investigated, and documented.

The project demonstrates a simplified security operations workflow from endpoint activity through SIEM detection and incident response.

Security Workflow

The overall workflow follows:

Build → Monitor → Simulate → Detect → Investigate → Respond → Document

Lab Scope

All security testing and attack simulations are performed only against systems owned and controlled within the isolated home-lab environment.
