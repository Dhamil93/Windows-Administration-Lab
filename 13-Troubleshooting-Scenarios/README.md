# Scenario 1: Network Connectivity Issue

## Problem
User reports inability to access websites.

## Investigation
Performed network diagnostics using:
- `ipconfig`
- `ping 8.8.8.8`
- `ping google.com`
- `nslookup google.com`

## Findings
- Wi-Fi adapter connected successfully.
- IPv4 address assigned correctly.
- DNS resolution functioning normally.
- Successful connectivity to Google and public DNS servers.
- No packet loss detected.

## Resolution
Network connectivity verified. No faults found during testing.

## Lessons Learned
Always verify IP configuration, DNS resolution, and connectivity in a logical troubleshooting sequence.

---

# Scenario 2: High CPU Usage

## Problem
System performance is slow.

## Investigation
Used Task Manager and Resource Monitor to identify processes consuming CPU resources and monitor overall system performance.

## Findings
- Overall CPU utilization remained around 11%.
- Performance Monitor, Desktop Window Manager, and Brave Browser showed the highest usage.
- No process was consuming excessive CPU resources.

## Resolution
No abnormal CPU utilization detected. System performance was within normal operating parameters.

## Lessons Learned
Resource Monitor provides detailed insight into process activity and helps identify applications affecting performance.

---

# Scenario 3: Windows Service Investigation

## Problem
Service not functioning as expected.

## Investigation
Reviewed Windows Services using `services.msc`. Checked the status of critical services including:
- Print Spooler
- Bluetooth Support Service
- Windows Time

## Findings
- Print Spooler service running.
- Bluetooth Support Service running.
- Windows Time service running.
- Startup configurations appeared correct.

## Resolution
All investigated services were functioning normally. No corrective action required.

## Lessons Learned
Verifying service status is an important step when diagnosing application and operating system issues.

---

# Scenario 4: Event Viewer Investigation

## Problem
System errors detected.

## Investigation
Opened Event Viewer and reviewed Warning and Error events under Windows Logs → System.

## Findings
- DistributedCOM Warning (Event ID 10016).
- TPM-WMI Error (Event ID 1803).
- No evidence of system instability or service failure resulting from these events.

## Resolution
Events documented for monitoring. No immediate remediation required because no user impact was observed.

## Lessons Learned
Event Viewer often contains informational warnings that require evaluation before determining whether action is necessary.

---

# Scenario 5: Disk Health Assessment

## Problem
Storage health verification required.

## Investigation
Executed:
```powershell
Get-PhysicalDisk
Get-Volume
```

Reviewed physical disk and volume health status.

## Findings
- WDC PC SN530 SSD reported healthy.
- Operational Status: OK.
- C: drive healthy.
- Recovery partition healthy.
- EFI partition healthy.

## Resolution
No storage issues identified. Disk and partitions operating normally.

## Lessons Learned
Routine disk health monitoring helps identify potential storage failures before they impact users.

---

# Scenario 6: Security Assessment

## Problem
Endpoint security verification required.

## Investigation
Reviewed:
- Windows Security Dashboard
- Microsoft Defender status
- TPM configuration
- Antivirus protection status

Executed:
```powershell
Get-MpComputerStatus
Get-Tpm
```

## Findings
- Microsoft Defender enabled.
- Antivirus signatures current.
- Real-time protection enabled.
- TPM present and operational.
- No active malware threats detected.

## Resolution
Security controls verified and functioning correctly.

## Lessons Learned
Regular security assessments help confirm endpoint protection and identify potential vulnerabilities before they become security incidents.
