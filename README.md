# Mini SOC Lab

## Overview

A lightweight defensive security laboratory built to demonstrate a basic Security Operations Center (SOC) workflow using Windows 11 and Microsoft Sysmon.

The project follows:

**Generate → Collect → Detect → Investigate → Report**

## Objectives

- Collect Windows security telemetry
- Monitor process creation using Sysmon
- Monitor network connections using Sysmon
- Detect authentication failures
- Detect local account creation
- Investigate PowerShell activity
- Correlate network events with processes
- Document findings from a SOC analyst perspective

## Lab Environment

- Operating System: Windows 11 Pro
- Monitoring Tool: Microsoft Sysmon v15.22
- Environment: Controlled local laboratory
- No public or third-party systems were targeted

## Detection Scenarios

| Scenario | Log Source | Event ID | Purpose |
|---|---|---:|---|
| Failed Logon | Windows Security | 4625 | Authentication failure detection |
| PowerShell Activity | Sysmon | 1 | Process creation investigation |
| Account Creation | Windows Security | 4720 | New account detection |
| Network Connection | Sysmon | 3 | Network/process correlation |

## SOC Workflow

```text
Generate
   ↓
Collect
   ↓
Detect
   ↓
Investigate
   ↓
Correlate
   ↓
Report
