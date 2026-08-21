# Wazuh Agent Setup

## Overview

The Wazuh Agent was configured on the Ubuntu endpoint to collect security-related telemetry and forward events to the Wazuh Manager for centralized monitoring and analysis.

## Lab Environment

| Component | Role |
|---|---|
| Ubuntu | Monitored endpoint |
| Wazuh Agent | Endpoint telemetry collection |
| Wazuh Manager | Centralized security monitoring |
| VirtualBox | Virtualization platform |

## Objective

Configure the Wazuh Agent on the Ubuntu endpoint and establish communication with the Wazuh Manager.

## Agent Installation

The Wazuh Agent was installed on the Ubuntu endpoint using the appropriate Wazuh installation procedure.

The agent configuration was then updated with the Wazuh Manager details required for communication.

## Agent Configuration

The Wazuh Agent configuration was reviewed to ensure that the endpoint was configured to communicate with the Wazuh Manager.

## Agent Service

The Wazuh Agent service was started and checked to confirm that it was running correctly.

Example verification:

```bash
sudo systemctl status wazuh-agentCommunication Verification

After starting the agent, communication with the Wazuh Manager was verified through the Wazuh management interface.

The endpoint appeared as an enrolled/connected agent in the Wazuh environment.

Result

Status: Successful

The Ubuntu endpoint was successfully configured with the Wazuh Agent and prepared for security-event monitoring.

Next Step

The next stage is to verify the complete Wazuh installation and confirm that security events from the endpoint are being received and processed by the Wazuh Manager.

Skills Demonstrated
Linux administration
Wazuh Agent configuration
SIEM endpoint onboarding
Service management
Security telemetry collection
Endpoint monitoring
