# Windows Backup Lab

## Overview

This lab demonstrates Windows backup, recovery, restore points, and recovery options used to protect systems against data loss and system failures.

---

## Objectives

- Review Windows Backup settings
- Review Backup and Restore features
- Review Recovery options
- Examine System Restore configuration
- Investigate available restore points
- Examine Volume Shadow Copy information

---

## Tools Used

- Windows Backup
- Backup and Restore
- Recovery
- System Protection
- PowerShell
- VSSAdmin

---

## Findings

The Windows Backup and Recovery assessment identified the following:

- Windows Backup is configured to synchronize settings with a Microsoft account.
- OneDrive folder synchronization is active.
- Application settings and preferences are being backed up.
- Backup and Restore (Windows 7) has not been configured.
- No local Windows backup sets were found.
- System Protection is disabled for the C: drive.
- No System Restore points currently exist.
- No Volume Shadow Copies were found on the system.
- Recovery tools are available, including Recovery Drive creation and System Restore options.

---

## Resolution

The backup and recovery configuration was reviewed using Windows Backup, Backup and Restore, Recovery tools, PowerShell, and VSSAdmin.

Actions performed:

1. Reviewed Windows Backup synchronization settings.
2. Verified OneDrive backup integration.
3. Examined Backup and Restore configuration.
4. Reviewed available recovery tools.
5. Checked System Protection status.
6. Investigated available restore points.
7. Checked Volume Shadow Copy availability.

No active backup jobs, restore points, or shadow copies were configured on the system at the time of assessment.

Recommendations include enabling System Protection and creating periodic restore points to improve recovery readiness.

---

## Lessons Learned

- Windows provides multiple recovery and backup mechanisms.
- OneDrive can be used as a cloud backup solution for files and settings.
- Backup and Restore (Windows 7) remains available for legacy backup operations.
- System Protection must be enabled before restore points can be created.
- Restore points help recover from software and configuration issues.
- Volume Shadow Copies support file recovery and backup operations.
- Regular backup validation is important to ensure recoverability during incidents.

---

## Backup Assessment Summary

### Backup Status

| Component | Status |
|------------|---------|
| OneDrive Backup | Enabled |
| Microsoft Account Sync | Enabled |
| Backup and Restore | Not Configured |
| System Protection | Disabled |
| Restore Points | None Found |
| Volume Shadow Copies | None Found |

### Risk Assessment

Medium

The system benefits from Microsoft account synchronization and OneDrive backup capabilities; however, local recovery features such as System Restore and Volume Shadow Copies are not currently configured.

---

## IT Support Talking Points

During this lab I reviewed Windows backup and recovery capabilities.

Tasks completed:

- Verified Windows Backup configuration.
- Assessed OneDrive synchronization status.
- Reviewed Backup and Restore functionality.
- Examined Recovery options.
- Investigated System Protection settings.
- Verified restore point availability.
- Reviewed Volume Shadow Copy status.
- Documented recovery readiness findings.

Tools Used:

- Windows Backup
- Backup and Restore
- Recovery
- System Protection
- PowerShell
- VSSAdmin

Skills Demonstrated:

- Backup Administration
- Disaster Recovery
- Business Continuity
- Windows Administration
- Technical Documentation
