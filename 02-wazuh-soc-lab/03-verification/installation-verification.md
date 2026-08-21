# Wazuh Installation & Communication Verification

## Overview

After deploying the Wazuh server and configuring the Wazuh Agent on the Ubuntu endpoint, the next step was to verify that the components were operating correctly and communicating with each other.

## Verification Objectives

The verification process focused on:

- Wazuh Manager availability
- Wazuh Agent service status
- Agent registration
- Agent connectivity
- Security event collection
- Endpoint visibility in the Wazuh dashboard

## Verification Workflow

```text
Wazuh Manager
      ↓
Wazuh Agent
      ↓
Agent Communication
      ↓
Security Events
      ↓
Wazuh Dashboard

Wazuh Manager Verification

The Wazuh Manager environment was checked to confirm that the server was operational.

Agent Verification

The Wazuh Agent service on the Ubuntu endpoint was checked to confirm that the service was running correctly.

Example:

sudo systemctl status wazuh-agent
Agent Connectivity

The Ubuntu endpoint was verified from the Wazuh environment to confirm that the agent was communicating with the Wazuh Manager.

Event Collection

Security events generated on the monitored endpoint were checked to verify that telemetry was being received by the Wazuh platform.

Result

Verification Status: Successful

The Wazuh environment was prepared for security-event generation, monitoring, and investigation.

Next Stage

The next stage of the lab is a controlled SSH attack simulation designed to generate authentication-related security events for detection and investigation.
