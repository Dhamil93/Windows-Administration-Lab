# 🎫 Ticket BL-001 - BitLocker Encryption Verification

## Overview

BitLocker is Microsoft's full disk encryption technology used to protect data by encrypting storage devices.

This lab demonstrates how to verify BitLocker status and review drive encryption settings.

---

# Ticket Information

| Field | Value |
|---------|---------|
| Ticket ID | BL-001 |
| Category | Endpoint Security |
| Priority | Medium |
| Status | Completed |
| Tool Used | BitLocker |

---

# Reported Request

Security team requests verification that endpoint encryption is enabled and operating correctly.

---

# Objective

Review BitLocker status and verify encryption settings on the workstation.

---

# Skills Demonstrated

- Endpoint Security
- Windows Administration
- BitLocker Management
- Security Compliance
- Technical Documentation

---

# Screenshots

Stored in the screenshots folder.

---

# Findings

The workstation was assessed to determine BitLocker encryption status and compliance with endpoint security requirements.

## BitLocker Configuration

The operating system drive (C:) was reviewed using both the BitLocker Control Panel and PowerShell.

Observed Status:

- Drive Capacity: 952.75 GB
- BitLocker Status: Disabled
- Protection Status: Off
- Encryption Method: None
- Conversion Status: Fully Decrypted
- Encryption Percentage: 0%
- Lock Status: Unlocked

---

## PowerShell Verification

The following administrative commands were executed:

```powershell
Get-BitLockerVolume
```

```powershell
manage-bde -status
```

Both commands confirmed that BitLocker protection is not currently enabled on the operating system drive.

---

## Security Assessment

The device is currently operating without full disk encryption.

No BitLocker key protectors were configured.

The system remains functional; however, data stored on the device would not be protected if the laptop were lost, stolen, or accessed by an unauthorized individual.
---# Resolution

BitLocker status was successfully verified using both graphical and command-line administration tools.

The operating system drive was confirmed to be fully decrypted with BitLocker protection disabled.

No configuration changes were made during this assessment.

Recommendation:

- Enable BitLocker on the operating system drive.
- Store recovery keys securely.
- Verify TPM functionality before deployment.
- Apply organizational encryption policies where applicable.

---

# Lessons Learned

This lab improved my understanding of Windows endpoint encryption and BitLocker administration.

Key lessons learned:

- BitLocker provides full disk encryption for Windows devices.
- Encryption helps protect data if a device is lost or stolen.
- Get-BitLockerVolume can be used to review BitLocker status using PowerShell.
- manage-bde -status provides detailed encryption information from the command line.
- Protection Status indicates whether BitLocker protection is active.
- Conversion Status indicates whether a drive is encrypted or decrypted.
- Security compliance reviews often include verification of endpoint encryption.

This exercise strengthened my understanding of endpoint security and encryption management.

---

# Real World Scenario

## Ticket BL-001

The Information Security team requested verification of endpoint encryption status before a security compliance review.

### Investigation

1. Opened BitLocker Drive Encryption settings.
2. Verified encryption configuration through the Control Panel.
3. Executed Get-BitLockerVolume.
4. Executed manage-bde -status.
5. Reviewed encryption and protection status.

### Findings

The operating system drive was fully decrypted.

BitLocker protection was disabled.

No encryption keys or protectors were configured.

### Resolution

The workstation was documented as non-encrypted.

A recommendation was made to enable BitLocker to improve endpoint security and compliance.


---

# Interview Questions

## What is BitLocker?

BitLocker is Microsoft's full disk encryption solution used to protect data stored on Windows devices.

---

## Why is BitLocker important?

It protects sensitive information if a device is lost, stolen, or accessed by unauthorized users.

---

## What command checks BitLocker status?

```powershell
Get-BitLockerVolume
```

or

```powershell
manage-bde -status
```

---

## What does "Fully Decrypted" mean?

The drive is not encrypted and BitLocker protection is not active.

---

## What does "Protection Off" mean?

BitLocker protection is disabled and data is not protected by disk encryption.

---

## What is a BitLocker Recovery Key?

A recovery key is used to regain access to an encrypted drive if normal authentication methods fail.
