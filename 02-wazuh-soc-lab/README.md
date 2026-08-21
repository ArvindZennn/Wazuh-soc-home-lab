# Wazuh SOC Lab

## Overview

This section documents the deployment and configuration of **Wazuh** as the SIEM and endpoint monitoring platform for the SOC home lab.

The lab demonstrates a simplified SOC workflow:

```text
Endpoint
    ↓
Wazuh Agent
    ↓
Wazuh Manager
    ↓
Security Events
    ↓
Detection
    ↓
Investigation
    ↓
Incident Response
```

## Lab Components

* Wazuh Manager
* Wazuh Agent
* Ubuntu endpoint
* Windows environment
* Oracle VirtualBox
* SSH
* Security event monitoring

## Lab Sections

### 01 — Wazuh Deployment

Deployment of the Wazuh virtual appliance and initial server setup.

### 02 — Agent Setup

Installation and configuration of the Wazuh agent on the Ubuntu endpoint.

### 03 — Installation Verification

Verification of Wazuh Manager, Agent, and endpoint communication.

### 04 — SSH Attack Simulation

Controlled SSH authentication attack performed against the lab endpoint.

### 05 — Detection & Analysis

Investigation of the generated security events and Wazuh alerts.

## SOC Workflow

```text
Deploy
  ↓
Configure
  ↓
Monitor
  ↓
Generate Security Event
  ↓
Detect
  ↓
Investigate
  ↓
Respond
  ↓
Document
```

## Objective

Build practical experience with SIEM deployment, endpoint monitoring, security event detection, log analysis, and incident investigation using Wazuh.
