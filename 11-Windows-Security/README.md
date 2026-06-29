# 🎫 Ticket WS-001 - Windows Security Assessment

## Overview

Windows Security provides built-in protection against malware, unauthorized access and security threats.

This lab demonstrates how to review endpoint security settings and verify protection status.

---

# Ticket Information

| Field | Value |
|---------|---------|
| Ticket ID | WS-001 |
| Category | Endpoint Security |
| Priority | High |
| Status | Completed |
| Tool Used | Windows Security |

---

# Reported Request

Security team requested verification of endpoint protection status.

---

# Objective

Review Windows Security configuration and verify protection settings.

---

# Skills Demonstrated

- Endpoint Security
- Windows Administration
- Microsoft Defender
- Security Compliance
- Security Assessment
- Technical Documentation

---

# Screenshots

Stored in the screenshots folder.

---

## Findings

The Windows Security assessment identified the following:

- Microsoft Defender Antivirus is installed and enabled.
- No active malware or threats were detected.
- Security intelligence definitions are up to date.
- TPM 2.0 is present, enabled, activated, and owned.
- Secure Boot is enabled.
- Core Isolation is available.
- Microsoft Defender Firewall is disabled for all network profiles.
- Cloud-delivered protection is disabled.
- Automatic sample submission is disabled.
- Device encryption is not currently enabled.
- Smart App Control and Exploit Protection features are available.

---

## Resolution

The security configuration was reviewed using Windows Security and PowerShell.

Actions performed:

1. Verified Microsoft Defender Antivirus status.
2. Confirmed antivirus signatures were current.
3. Reviewed Protection History for security alerts.
4. Verified TPM functionality and readiness.
5. Confirmed Secure Boot status.
6. Reviewed Firewall configuration.
7. Reviewed App & Browser Control protections.
8. Reviewed Microsoft Defender preferences.

No malware was detected during the assessment.

Firewall and cloud-based protection settings were identified as areas requiring remediation to improve endpoint security posture.

---

## Lessons Learned

- Windows Security provides a centralized dashboard for endpoint protection.
- TPM and Secure Boot are important security controls for modern Windows systems.
- Microsoft Defender Antivirus can remain operational even when other protection features are disabled.
- Firewall protection should remain enabled whenever possible.
- Cloud-delivered protection improves malware detection capabilities.
- PowerShell provides detailed visibility into Defender and TPM configurations.
- Security reviews should be performed regularly to identify configuration weaknesses.

---

# Real World Scenario

## Ticket WS-001

The security team requested verification that endpoint protection controls were functioning correctly.

### Investigation

1. Review Microsoft Defender status.
2. Verify antivirus protection.
3. Review firewall configuration.
4. Verify TPM availability.
5. Review endpoint security settings.

---

## Security Audit Notes

### Positive Findings

- Microsoft Defender Antivirus Enabled
- No Active Threats Detected
- Security Definitions Up To Date
- TPM Enabled And Operational
- Secure Boot Enabled

### Risks Identified

- Microsoft Defender Firewall Disabled
- Cloud-Delivered Protection Disabled
- Automatic Sample Submission Disabled
- Device Encryption Not Enabled

### Risk Level

Medium

The system has core security protections enabled, but several recommended Microsoft Defender security controls are disabled and should be reviewed.

---

# Interview Questions

## What is Microsoft Defender?

Microsoft Defender is the built-in antivirus and endpoint protection solution in Windows.

---

## What is TPM?

Trusted Platform Module (TPM) is a hardware security component used for encryption and secure authentication.

---

## Why is Secure Boot important?

Secure Boot prevents unauthorized software from loading during startup.

---

## What command checks Defender status?

```powershell
Get-MpComputerStatus
```

---

## What command checks TPM status?

```powershell
Get-Tpm
```

---

## Why is Windows Security important?

It provides protection against malware, ransomware, phishing, unauthorized access and security threats.

---

## SOC Analyst Talking Points

During this lab I performed a Windows endpoint security assessment using Microsoft Defender Security Center and PowerShell.

Tasks completed:

- Verified antivirus protection status.
- Reviewed endpoint protection history.
- Assessed firewall configuration.
- Validated TPM readiness.
- Confirmed Secure Boot configuration.
- Reviewed Defender preferences and security settings.
- Identified security gaps and documented remediation recommendations.

Tools Used:

- Windows Security
- Microsoft Defender
- PowerShell
- TPM Management
- Secure Boot Verification

Skills Demonstrated:

- Endpoint Security
- Security Monitoring
- Security Assessment
- Windows Administration
- Technical Documentation
