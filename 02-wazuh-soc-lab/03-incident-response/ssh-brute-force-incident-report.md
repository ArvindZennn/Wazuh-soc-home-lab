# SSH Brute-Force Incident Report

## 1. Incident Overview

| Field | Details |
|---|---|
| Incident Type | SSH Brute-Force Simulation |
| Environment | Isolated SOC Home Lab |
| Detection Platform | Wazuh |
| Target | Ubuntu Endpoint |
| Status | Investigated |
| Severity | Lab Assessment |

## 2. Executive Summary

A controlled SSH brute-force simulation was performed against an Ubuntu endpoint within the isolated SOC home lab.

The resulting authentication events were collected by the Wazuh Agent and analyzed through the Wazuh monitoring environment.

## 3. Attack Activity

The simulation generated repeated unsuccessful SSH authentication attempts.

These events created authentication telemetry that could be analyzed by the SIEM.

## 4. Detection

Wazuh detected the authentication activity and generated security alerts based on the observed events.

## 5. Investigation

The alert was investigated by reviewing:

- Authentication events
- Event timestamps
- Source information
- Target endpoint
- Detection information
- Related logs

## 6. Findings

The investigation confirmed that the observed activity matched the behavior expected from the controlled SSH brute-force simulation.

## 7. Response

For this controlled lab exercise, the primary objective was detection and investigation rather than production containment.

Potential defensive responses include:

- Blocking suspicious sources
- Strengthening SSH authentication
- Using key-based authentication
- Disabling unnecessary password authentication
- Monitoring repeated authentication failures
- Implementing appropriate access controls

## 8. Lessons Learned

This exercise demonstrated the relationship between:

```text
Attack Activity
      ↓
Endpoint Logs
      ↓
Agent Telemetry
      ↓
SIEM Detection
      ↓
SOC Investigation
      ↓
Incident Documentation

9. Recommendations

For a production environment:

Use strong authentication controls
Prefer SSH key-based authentication
Restrict SSH exposure
Monitor authentication failures
Implement appropriate firewall controls
Continuously monitor security events
Maintain incident-response procedures
10. Conclusion

The exercise demonstrated a complete defensive security workflow from controlled attack simulation through SIEM detection, investigation, and incident documentation.

All activity documented in this report was performed within an authorized and isolated home-lab environment.
