# 🎫 Ticket EV-001 - Unexpected System Restart Investigation

## Overview

This project demonstrates how to use Windows Event Viewer to investigate an unexpected system restart.

Event Viewer is an essential Windows administration tool used by IT Support Engineers to diagnose operating system, hardware and application issues.

---

# Ticket Information

| Field | Value |
|------|------|
| Ticket ID | EV-001 |
| Category | Windows Operating System |
| Priority | Medium |
| Status | Completed |
| Tool Used | Event Viewer |

---

# Reported Issue

**User reports that the computer restarted unexpectedly during normal use.**

---

# Objective

Investigate the Windows Event Logs to determine whether the restart was caused by hardware, drivers, Windows, or an application.

---

# Investigation Steps

1. Open Event Viewer.
2. Navigate to **Windows Logs**.
3. Review the **System** log.
4. Filter **Critical**, **Error**, and **Warning** events.
5. Review Event IDs and event descriptions.
6. Document findings.
7. Verify whether the issue is recurring.

---

# Screenshots

Screenshots are stored in the `screenshots` folder.

---

# Findings

During the investigation several system events were identified.

## Event 10010

**Source:** DistributedCOM

**Level:** Error

The event indicated that a COM server failed to register within the required timeout period.

This type of event is commonly observed during Windows startup or when applications take longer than expected to initialize.

---

## Event 7043

**Source:** Service Control Manager

This event indicates that a Windows service encountered an issue during startup or shutdown.

---

## Security Events

The Security log recorded successful security auditing events including:

- Event ID 5061 (Cryptographic Operation)
- Event ID 4672 (Special Logon)
- Event ID 5379 (Credential Manager)
- Event ID 4798 (User Account Management)

These indicate that Windows security auditing is functioning correctly.

---

No evidence of hardware failure or repeated system crashes was identified during this investigation.

---

# Resolution

The investigation determined that the DistributedCOM errors were isolated timeout events.

No hardware failures or critical operating system issues were detected.

The system continued to operate normally after reviewing the logs.

No corrective action was required.

Recommendation:

Continue monitoring Event Viewer for recurring errors or patterns that may indicate a developing issue.

---

# Lessons Learned


This lab improved my understanding of Windows Event Viewer and how IT Support Engineers investigate operating system events.

Key lessons include:

- Windows records application, security and system events in Event Viewer.
- Event IDs help identify specific operating system activities.
- Not every Error event requires immediate remediation.
- Filtering logs helps administrators quickly identify important events.
- Security logs provide valuable auditing information.
---

# Interview Questions

## What is Event Viewer?

Event Viewer is a Windows administrative tool used to monitor and troubleshoot system, application and security events.

---

## What is an Event ID?

An Event ID is a unique number assigned to a Windows event that helps identify a specific activity or issue.

---

## What does Event ID 10010 mean?

Event ID 10010 is a DistributedCOM timeout event indicating that a COM server did not register within the expected time.

It is commonly observed during system startup and is not always indicative of a serious problem.

---

## Why are Security logs important?

Security logs record authentication events, privilege usage and auditing information used to monitor system security.
---

# Skills Demonstrated

- Windows Administration
- Event Viewer
- Desktop Support
- Incident Investigation
- Troubleshooting
- Root Cause Analysis
- Technical Documentation
