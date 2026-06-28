# 🎫 Ticket PS-001 - System Administration Using PowerShell

## Overview

PowerShell is a command-line shell and scripting language used to automate administrative tasks and manage Windows systems.

This lab demonstrates common PowerShell commands used by IT Support Engineers and Systems Administrators.

---

# Ticket Information

| Field | Value |
|---------|---------|
| Ticket ID | PS-001 |
| Category | System Administration |
| Priority | Medium |
| Status | Completed |
| Tool Used | Windows PowerShell |

---

# Reported Request

IT Support requires system information and administrative verification using PowerShell.

---

# Objective

Use PowerShell commands to gather system information, identify users, review network settings and perform administrative tasks.

---

# Skills Demonstrated

- Windows Administration
- PowerShell Fundamentals
- System Inventory
- Network Troubleshooting
- User Management
- Technical Documentation

---

# Screenshots

Stored in the screenshots folder.

---

# Findings

The workstation was investigated using PowerShell administrative commands.

## System Information

The device was successfully inventoried using Get-ComputerInfo.

System Details:

- Device Manufacturer: Acer
- Operating System: Windows 11 Pro
- Windows Version: 25H2
- BIOS Manufacturer: Insyde Corp.
- BIOS Version: V1.11
- BIOS Release Date: 30 September 2022

The workstation is operating with UEFI firmware and Windows Professional edition.

---

## Local User Accounts

The following local accounts were identified:

- damil (Enabled)
- Administrator (Disabled)
- Guest (Disabled)
- DefaultAccount (Disabled)
- WDAGUtilityAccount (Disabled)
- WsiAccount (Disabled)

Only one active user account was identified during the investigation.

---

## Network Adapters

The following adapters were detected:

### Active Adapters

- Intel(R) Wi-Fi 6 AX200 160MHz
- Hyper-V Virtual Ethernet Adapter

### Inactive Adapters

- TunnelBear Adapter V9
- Bluetooth Network Connection

The primary network connection was operating through the Intel Wi-Fi adapter.

---

## IP Address Information

PowerShell successfully displayed IPv4 and IPv6 addressing information.

Key Findings:

- Wi-Fi adapter assigned a valid IP address
- IPv6 enabled
- Hyper-V virtual networking present
- Multiple interfaces configured correctly

No addressing issues were identified.

---

## Installed Updates

The following Windows updates were identified:

- KB5092427
- KB5054156
- KB5095093
- KB5095182

Installed updates indicate that the workstation is receiving security and system updates.

No missing update concerns were observed.

---

# Resolution

PowerShell commands were successfully used to investigate system configuration, local accounts, networking and installed updates.

System inventory was collected successfully.

User accounts were reviewed and verified.

Network adapters and IP addressing were functioning correctly.

Windows updates were present and current.

No issues requiring remediation were identified during this investigation.

---

# Lessons Learned

This lab improved my understanding of Windows PowerShell administration.

Key lessons learned:

- Get-ComputerInfo provides detailed hardware and operating system information.
- Get-LocalUser displays local user accounts.
- Get-LocalGroup displays security groups.
- Get-NetAdapter displays network adapter status.
- Get-NetIPAddress displays IP addressing information.
- Get-HotFix displays installed Windows updates.
- PowerShell can retrieve administrative information much faster than graphical tools.

This lab strengthened my understanding of Windows administration and PowerShell-based troubleshooting.

---

# Real World Scenario

## Ticket PS-001

A Service Desk analyst receives a ticket regarding workstation configuration verification.

### Investigation

1. Collected system information using Get-ComputerInfo.
2. Reviewed local user accounts using Get-LocalUser.
3. Verified network adapters using Get-NetAdapter.
4. Reviewed IP addressing using Get-NetIPAddress.
5. Confirmed installed updates using Get-HotFix.

### Findings

The workstation was correctly configured.

Only one active local user account was present.

Network connectivity and adapter configuration appeared normal.

Windows updates were installed successfully.

### Resolution

No configuration issues were identified.

The workstation remained compliant with standard operational requirements.

---

# Interview Questions

## What is PowerShell?

PowerShell is a command-line shell and scripting language used for system administration and automation.

---

## What does Get-ComputerInfo do?

Displays detailed operating system and hardware information.

---

## What does Get-LocalUser do?

Lists local user accounts on a workstation.

---

## What does Get-NetAdapter do?

Displays network adapters and their operational status.

---

## What does Get-NetIPAddress do?

Displays IPv4 and IPv6 address configuration.

---

## What does Get-HotFix do?

Displays installed Windows updates and security patches.

---

## Why is PowerShell important for IT administrators?

PowerShell enables automation, configuration management and troubleshooting across Windows systems.
