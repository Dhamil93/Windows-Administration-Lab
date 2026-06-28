# 🎫 Ticket WS-001 - Print Services Investigation

## Overview

Windows Services are background processes that support operating system functionality and application operations.

This lab demonstrates how to investigate and manage Windows services using the Services Management Console.

---

# Ticket Information

| Field | Value |
|---------|---------|
| Ticket ID | WS-001 |
| Category | Windows Services |
| Priority | Medium |
| Status | Completed |
| Tool Used | Services.msc |

---

# Reported Issue

User reports that printing functionality is unavailable.

---

# Objective

Investigate critical Windows services and understand their purpose, startup type and operational status.

---

# Services Reviewed

- Print Spooler
- Windows Update
- Windows Defender
- DHCP Client
- DNS Client
- Windows Time

---

# Skills Demonstrated

- Windows Administration
- Desktop Support
- Service Management
- Troubleshooting
- Technical Documentation

---

# Screenshots

Stored in the screenshots folder.

---

# Findings

The following critical Windows services were reviewed during this investigation.

## Print Spooler

Status: Running

Startup Type: Automatic

Purpose:

Manages print jobs and communication between Windows and installed printers.

---

## DHCP Client

Status: Running

Startup Type: Automatic

Purpose:

Obtains and renews IP addresses from DHCP servers and registers DNS records.

---

## DNS Client

Status: Running

Startup Type: Automatic

Purpose:

Resolves hostnames into IP addresses and caches DNS queries.

---

## Windows Update

Status: Running

Startup Type: Manual

Purpose:

Downloads and installs Windows updates and security patches.

---

## Windows Time

Status: Running

Startup Type: Manual

Purpose:

Synchronizes system time with configured time sources.

---

## Windows Defender Firewall

Status: Running

Startup Type: Automatic

Purpose:

Provides network protection by filtering inbound and outbound traffic.

---

No service failures were observed during the investigation.

All reviewed services were functioning normally.

---

# Technical Analysis

The services reviewed support critical operating system functionality.

The DHCP Client and DNS Client services are essential for network connectivity. If either service stops, users may experience internet or network access issues.

The Print Spooler service is required for printing operations. If stopped, users will be unable to print documents.

Windows Defender Firewall provides endpoint protection and should remain enabled unless alternative security controls are in place.

Windows Update ensures the operating system receives security patches and feature updates.

The Windows Time service maintains accurate system time, which is important for authentication, certificates and domain services.

All services reviewed were operating as expected.

---

# Resolution

The investigation determined that all reviewed Windows services were operating normally.

The following services were verified:

- Print Spooler
- DHCP Client
- DNS Client
- Windows Update
- Windows Time
- Windows Defender Firewall

All services were running successfully and configured with appropriate startup settings.

No service failures, crashes or interruptions were identified.

No corrective action was required.

Recommendation:

Continue monitoring critical Windows services and investigate any future service failures through the Services console and Event Viewer.

---

# Real World Scenario

## Ticket WS-001

User reports that documents are not printing.

### Investigation

1. Open Services (services.msc)
2. Locate Print Spooler
3. Verify service status
4. Restart the service if stopped
5. Check printer connectivity
6. Attempt a test print

### Findings

The Print Spooler service was running normally.

No service-related issues were identified.

### Resolution

No action required.

Printer troubleshooting would continue at the device or driver level if the issue persists.

---

# Interview Questions

## What is a Windows Service?

A Windows Service is a background process that runs independently of user interaction and supports operating system or application functionality.

---

## What does the Print Spooler service do?

It manages print jobs and communication between Windows and installed printers.

---

## What happens if the DHCP Client service stops?

The computer may fail to obtain an IP address automatically and lose network connectivity.

---

## What does the DNS Client service do?

It resolves hostnames into IP addresses and caches DNS queries for faster lookups.

---

## Why is Windows Time important?

Accurate system time is required for authentication, certificates, security logs and domain communication.

---

## How do you open Services?

Windows + R

services.msc

---

# Lessons Learned
During this lab I gained practical experience working with Windows Services and understanding their role in operating system functionality.

Key lessons learned:

- Windows Services run in the background and support critical system functions.
- Print Spooler is required for printing operations.
- DHCP Client is responsible for obtaining IP addresses from network DHCP servers.
- DNS Client resolves hostnames into IP addresses.
- Windows Defender Firewall helps secure the system from unauthorized network access.
- Windows Update is responsible for installing security and feature updates.
- Windows Time maintains accurate system time synchronization.

This lab improved my understanding of how IT Support Engineers investigate service-related issues and verify service health.
