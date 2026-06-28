# 🎫 Ticket CMD-001 - Network Connectivity Investigation

## Overview

Command Prompt is a Windows administration tool used for troubleshooting network, system and connectivity issues.

This lab demonstrates the use of common networking commands used by IT Support Engineers to diagnose network problems and verify connectivity.

---

# Ticket Information

| Field | Value |
|---------|---------|
| Ticket ID | CMD-001 |
| Category | Network Troubleshooting |
| Priority | Medium |
| Status | In Progress |
| Tool Used | Command Prompt |

---

# Reported Issue

User reports intermittent internet connectivity and inability to access websites.

---

# Objective

Use Command Prompt tools to investigate network connectivity and system configuration.

---

# Investigation Steps

1. Identify device hostname.
2. Review IP configuration.
3. Verify internet connectivity.
4. Test DNS resolution.
5. Analyze network routes.
6. Review active connections.
7. Gather system information.
8. Document findings.

---

# Screenshots

Stored in the screenshots folder.

---

# Findings

The system network configuration was reviewed using Windows Command Prompt diagnostic tools.

## Hostname

Hostname identified:

ATILOLA-DAMILAR

---

## IP Configuration

The active wireless adapter was identified as:

Intel(R) Wi-Fi 6 AX200 160MHz

Network Configuration:

- IPv4 Address: 192.168.68.50
- Subnet Mask: 255.255.252.0
- Default Gateway: 192.168.68.1
- DHCP Enabled: Yes
- DHCP Server: 192.168.68.1
- DNS Servers:
  - 192.168.1.254
  - 192.168.68.1

Additional adapters identified:

- TunnelBear Adapter V9
- Hyper-V Virtual Ethernet Adapter
- Bluetooth Personal Area Network Adapter

---

## Connectivity Testing

Connectivity to external resources was tested using:

ping google.com

Results:

- Packets Sent: 4
- Packets Received: 4
- Packets Lost: 0
- Packet Loss: 0%

Latency Results:

- Minimum: 8ms
- Maximum: 12ms
- Average: 9ms

Internet connectivity was functioning normally.

---

## DNS Resolution

DNS resolution was tested using:

nslookup google.com

DNS Server:

192.168.1.254

Google domain names were successfully resolved to multiple IPv4 and IPv6 addresses.

DNS functionality was operating correctly.

---

## Active Network Connections

Netstat identified:

- Multiple listening services
- Active HTTPS connections using port 443
- Local listening ports including 135 and 445
- Established outbound connections to Microsoft and external cloud services

No abnormal network activity was identified during the investigation.

---

## System Information

Operating System:

Microsoft Windows 11 Pro

System Manufacturer:

Acer

System Model:

Swift SF314-42

Processor:

AMD Ryzen 5 4500U with Radeon Graphics

Installed Memory:

8 GB RAM

System Type:

x64-based PC

The device was operating normally during testing.

---

# Resolution

Network connectivity and system configuration were successfully verified using Command Prompt tools.

The workstation received a valid IP address from DHCP and successfully communicated with external internet resources.

DNS resolution was functioning correctly and active network connections appeared normal.

No connectivity issues were identified during testing.

No corrective action was required.

---

# Lessons Learned

This lab improved my understanding of Windows command-line troubleshooting and network diagnostics.

Key lessons learned:

- hostname identifies the computer name used on the network.
- ipconfig displays network configuration information.
- ipconfig /all provides detailed adapter configuration, DHCP and DNS information.
- ping verifies internet connectivity and measures latency.
- nslookup validates DNS resolution.
- netstat displays active connections and listening services.
- systeminfo provides operating system and hardware information.

This lab strengthened my ability to diagnose connectivity issues using native Windows troubleshooting tools.

---

# Real World Scenario

## Ticket CMD-001

A user reported intermittent internet connectivity and difficulty accessing websites.

### Investigation

1. Verified network configuration using ipconfig /all.
2. Confirmed valid DHCP assignment.
3. Tested internet connectivity using ping.
4. Verified DNS functionality using nslookup.
5. Reviewed active network connections using netstat.
6. Gathered device information using systeminfo.

### Findings

The workstation received a valid IP address and successfully communicated with external resources.

DNS resolution was functioning normally.

No packet loss was detected.

### Resolution

No network faults were identified.

The user was advised to continue monitoring connectivity and report any recurring issues.

---

# Interview Questions

## What command shows your IP address?

ipconfig

---

## What command shows detailed network information?

ipconfig /all

---

## What does ping test?

Network connectivity and latency between devices.

---

## What does nslookup do?

Tests DNS resolution and converts hostnames into IP addresses.

---

## What does netstat -ano display?

Active network connections, listening ports and process IDs.

---

## What does a 0% packet loss result indicate?

All packets were successfully transmitted and received without loss.

---

## What is DHCP?

Dynamic Host Configuration Protocol automatically assigns IP addresses to devices on a network.

---
# Skills Demonstrated

- Windows Administration
- Network Troubleshooting
- Command Line Operations
- DNS Troubleshooting
- Connectivity Testing
- Technical Documentation
