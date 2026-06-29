# 🎫 Ticket RDP-001 - Remote Desktop Configuration Review

## Overview

Remote Desktop allows administrators and support personnel to remotely access and manage Windows systems.

This lab demonstrates how to review Remote Desktop settings and verify remote access configuration.

---

# Ticket Information

| Field | Value |
|---------|---------|
| Ticket ID | RDP-001 |
| Category | Remote Access |
| Priority | Medium |
| Status | In Progress |
| Tool Used | Remote Desktop |

---

# Reported Request

A user requires confirmation that Remote Desktop is configured correctly for remote support purposes.

---

# Objective

Review Remote Desktop configuration and verify remote access settings.

---

# Skills Demonstrated

- Remote Administration
- Windows Administration
- Remote Desktop Configuration
- User Access Management
- Technical Documentation

---

# Screenshots

Stored in the screenshots folder.

---

# Findings

Remote Desktop configuration was reviewed using Windows Settings, System Properties and PowerShell.

## Device Information

Computer Name:

- ATILOLA-DAMILAR

This hostname would be used by support personnel when attempting a Remote Desktop connection.

---

## Remote Desktop Status

Remote Desktop was found to be disabled.

Observed Settings:

- Remote Desktop: Off
- Remote Assistance: Enabled
- Network Level Authentication (NLA): Available
- Default RDP Port: 3389

---

## Port Verification

The following PowerShell command was executed:

```powershell
Test-NetConnection -ComputerName localhost -Port 3389
```

Results:

- PingSucceeded: True
- TcpTestSucceeded: False

The RDP port was not actively listening because Remote Desktop was disabled.

---

## Firewall Review

Remote Desktop firewall rules were identified.

Observed Status:

- Remote Desktop TCP Rule: Disabled
- Remote Desktop UDP Rule: Disabled

Firewall configuration matched the current Remote Desktop configuration.

---

## Security Assessment

The workstation was not configured to accept Remote Desktop connections.

No unauthorized remote access exposure was identified.

The system remains secure from inbound RDP connections until Remote Desktop is enabled.

---

# Resolution

Remote Desktop configuration was successfully reviewed.

Testing confirmed that:

- Remote Desktop was disabled.
- Firewall rules associated with Remote Desktop were disabled.
- Port 3389 was not listening.
- Remote Assistance remained available.

No configuration issues were identified.

The workstation is operating as expected based on its current remote access configuration.

If remote administration is required in the future, Remote Desktop can be enabled through Windows Settings or System Properties.

---

# Lessons Learned

This lab improved my understanding of Windows Remote Desktop administration.

Key lessons learned:

- Remote Desktop uses TCP port 3389.
- Remote Desktop must be enabled before remote connections can be established.
- Firewall rules are automatically linked to Remote Desktop status.
- Test-NetConnection can be used to verify service availability.
- Remote Assistance and Remote Desktop are different technologies.
- Computer names are required when initiating RDP sessions.
- Network Level Authentication improves Remote Desktop security.

This exercise strengthened my understanding of remote administration and access troubleshooting.

---

# Real World Scenario

## Ticket RDP-001

A remote employee reported that IT Support could not connect to their workstation using Remote Desktop.

### Investigation

1. Verified computer name.
2. Reviewed Remote Desktop settings.
3. Tested TCP port 3389.
4. Reviewed firewall configuration.
5. Confirmed remote access status.

### Findings

Remote Desktop was disabled.

Firewall rules associated with Remote Desktop were also disabled.

Port 3389 was not accepting inbound connections.

### Resolution

Remote Desktop was identified as disabled by design.

No faults were detected.

If remote administration becomes necessary, Remote Desktop can be enabled and firewall rules activated.

---

# Interview Questions

## What is Remote Desktop?

Remote Desktop allows users and administrators to remotely connect to and manage Windows systems.

---

## What port does Remote Desktop use?

TCP Port 3389.

---

## How can you test Remote Desktop connectivity?

```powershell
Test-NetConnection -Port 3389
```

---

## Why might Remote Desktop fail?

- Disabled Remote Desktop
- Firewall blocking traffic
- Incorrect permissions
- Network connectivity issues
- Port 3389 blocked

---

## What is the difference between Remote Desktop and Remote Assistance?

Remote Desktop provides full remote access, while Remote Assistance allows collaborative troubleshooting with the user's participation.
