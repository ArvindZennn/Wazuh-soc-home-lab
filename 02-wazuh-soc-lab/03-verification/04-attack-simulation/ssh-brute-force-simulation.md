# SSH Brute-Force Attack Simulation

## Overview

A controlled SSH authentication attack was performed against the Ubuntu endpoint in the isolated home lab.

The purpose of the simulation was to generate authentication events that could be collected and analyzed by Wazuh.

> All testing was performed against systems owned and controlled within the lab environment.

## Objective

The objectives of this simulation were to:

- Generate failed SSH authentication events
- Observe the resulting endpoint logs
- Verify Wazuh event collection
- Trigger security detection
- Analyze the generated alert

## Attack Scenario

The test simulated repeated unsuccessful SSH authentication attempts against the lab endpoint.

```text
Test System
     |
     | SSH authentication attempts
     ↓
Ubuntu Endpoint
     |
     | Authentication logs
     ↓
Wazuh Agent
     |
     ↓
Wazuh Manager
     |
     ↓
Security Alert

Test Environment
Component	Role
Ubuntu	Target endpoint
SSH	Authentication service
Wazuh Agent	Telemetry collection
Wazuh Manager	Detection and analysis
Attack Execution

The controlled authentication test was performed against the lab SSH service.

The objective was not exploitation of a real system, but generation of realistic authentication telemetry for defensive analysis.

Expected Security Events

Repeated failed authentication attempts were expected to generate SSH-related security events.

These events were then forwarded to the Wazuh monitoring environment.

Result

The simulation successfully generated authentication-related security events for subsequent detection and investigation.

Next Stage

The generated events were analyzed in Wazuh to determine how the SIEM detected and classified the activity.
