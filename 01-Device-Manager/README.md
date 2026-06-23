
# 🖥️ Device Manager Lab

## Overview

Device Manager is one of the most important tools used by IT Support Engineers and Desktop Support Technicians.

It allows administrators to:

- View installed hardware
- Manage device drivers
- Identify hardware problems
- Troubleshoot Windows devices
- Enable or disable hardware
- Update drivers

This lab documents my hands-on experience using Windows Device Manager.

---

# 🎯 Lab Objectives

By completing this lab I will learn how to:

- Open Device Manager
- Identify installed hardware
- View driver information
- Investigate device properties
- Identify driver problems
- Understand Hardware IDs
- Review device events

---

# 🖥️ Lab Environment

| Item | Details |
|------|---------|
| Operating System | Windows 11 |
| Device | *(Enter your laptop model)* |
| Tool | Windows Device Manager |

---

# 📋 Tasks Completed

- [ ] Open Device Manager
- [ ] Review Display Adapters
- [ ] Review Disk Drives
- [ ] Review Network Adapters
- [ ] Review Processors
- [ ] Review USB Controllers
- [ ] View Driver Properties
- [ ] View Hardware IDs
- [ ] View Device Events

---

# 📸 Screenshots

This folder will contain screenshots taken during the lab.

```
screenshots/
```

Example:

- Device Manager Overview
- Display Adapter
- Network Adapter
- Driver Tab
- Events Tab
- Hardware IDs

---

# 🔍 What I Learned

During this lab I explored Windows Device Manager and gained practical experience identifying and managing hardware devices installed on a Windows computer.

## Hardware Identified

### Processor

- AMD Ryzen 5 4500U with Radeon Graphics

### Graphics Adapter

- AMD Radeon(TM) Graphics

### Storage

- WDC PC SN530 SDBPNPZ-1T00-1014 NVMe SSD

### Network

- Intel(R) Wi-Fi 6 AX200 160MHz
- Bluetooth Personal Area Network
- WAN Miniport Adapters
- TunnelBear Virtual Adapter

### USB

- USB Root Hub (USB 3.0)
- USB Composite Device
- AMD USB 3.10 eXtensible Host Controller

---

## Key Observations

- Windows successfully detected all installed hardware.
- No warning icons or hardware errors were present.
- All major hardware components were functioning correctly.
- Network adapters included physical, virtual and VPN interfaces.
- USB devices were managed through Windows USB Controllers.

---


# 🛠 Skills Demonstrated

- Windows Administration
- Desktop Support
- Driver Management
- Hardware Troubleshooting
- Device Diagnostics
- Windows 11 Administration
- Technical Documentation

---

# Technical Analysis

The system contains an AMD Ryzen 5 4500U processor with integrated Radeon Graphics, making it suitable for everyday productivity, virtualization, and IT support labs.

The system uses a Western Digital NVMe SSD, providing fast boot times and improved application performance.

Networking is handled by an Intel Wi-Fi 6 AX200 adapter, supporting modern wireless standards.

The presence of the TunnelBear Virtual Adapter demonstrates how VPN software installs virtual network interfaces within Windows.

No hardware conflicts or driver issues were detected during this inspection.
---

# Interview Questions

### What is Device Manager?

Device Manager is a Windows administrative tool used to manage hardware devices and device drivers.

---

### Why is Device Manager important?

It allows administrators to:

- Install drivers
- Update drivers
- Disable hardware
- Enable hardware
- Diagnose hardware issues

---

### What does a yellow warning icon mean?

A driver or hardware problem exists.

---

### What is a Hardware ID?

A unique identifier used by Windows to identify hardware devices and locate the correct driver.

---

### What is a Device Driver?

Software that allows Windows to communicate with hardware devices.

---

# Real World Scenario

A user reports that Wi-Fi is no longer working.

Troubleshooting steps:

1. Open Device Manager.
2. Expand Network Adapters.
3. Verify the Wi-Fi adapter appears.
4. Check for warning icons.
5. Review Driver Properties.
6. Update or reinstall the driver if necessary.
7. Restart the computer.
8. Test network connectivity.

Result:

This process helps isolate whether the issue is caused by hardware, drivers or Windows configuration.

---

# 📚 References

Microsoft Learn

https://learn.microsoft.com/windows/

Microsoft Device Manager Documentation

https://learn.microsoft.com/windows-hardware/drivers/
