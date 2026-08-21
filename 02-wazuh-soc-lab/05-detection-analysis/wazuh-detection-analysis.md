# Wazuh Detection & SOC Analysis

## Overview

Following the controlled SSH attack simulation, the generated security events were analyzed using Wazuh.

This stage demonstrates the core SOC workflow of detecting, triaging, and investigating suspicious authentication activity.

## Detection Workflow

```text
SSH Attack Simulation
        ↓
Failed Authentication Events
        ↓
Wazuh Agent
        ↓
Wazuh Manager
        ↓
Detection Rule
        ↓
Security Alert
        ↓
SOC Investigation

Detection

Wazuh received the authentication events generated during the SSH simulation and generated security alerts based on the observed activity.

Alert Analysis

The alert was reviewed to understand:

Source information
Destination endpoint
Authentication activity
Event timestamp
Detection severity
Detection rule
Relevant log information
Investigation

The activity was analyzed to determine whether the authentication failures represented suspicious behavior.

Repeated failed authentication attempts were treated as suspicious activity within the controlled lab environment.

Findings

The investigation demonstrated how endpoint authentication telemetry can be collected and correlated by a SIEM platform to identify potentially malicious activity.

SOC Analyst Perspective

The investigation followed a simplified workflow:

Identify the alert
Review event details
Examine authentication activity
Determine the nature of the activity
Document findings
Recommend appropriate response actions
Result

The Wazuh environment successfully provided visibility into the simulated SSH authentication activity.

Next Stage

The findings from this investigation were documented as an incident-response report.
