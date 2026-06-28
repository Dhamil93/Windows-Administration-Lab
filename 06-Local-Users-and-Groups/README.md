# 🎫 Ticket LU-001 - Local User Account Investigation

## Overview

Local Users and Groups is a Windows administrative tool used to manage local user accounts and security groups.

This lab demonstrates how to review local user accounts, group memberships and administrative privileges.

---

# Ticket Information

| Field | Value |
|---------|---------|
| Ticket ID | LU-001 |
| Category | User Administration |
| Priority | Medium |
| Status | Completed |
| Tool Used | Local Users and Groups |

---

# Reported Request

A manager requests verification of local user accounts and administrator access on a Windows workstation.

---

# Objective

Review local users and groups and identify accounts with administrative privileges.

---

# Skills Demonstrated

- User Management
- Access Control
- Windows Administration
- Desktop Support
- Technical Documentation

---

# Screenshots

Stored in the screenshots folder.

---

# Findings

The Local Users and Groups console was reviewed.

## Local Accounts Identified

- Administrator
- DefaultAccount
- Guest
- Local User Accounts

---

## Groups Reviewed

- Administrators
- Users
- Remote Desktop Users

---

## Administrative Access

The Administrators group was reviewed to identify accounts with elevated privileges.

Only authorized accounts should maintain administrative access.

---

No unauthorized local accounts were identified during this review.

---

# Resolution

Local user accounts and security groups were reviewed successfully.

Administrative access was verified through the Administrators group.

No unauthorized accounts or unexpected group memberships were identified.

No corrective action was required.

---

# Lessons Learned

This lab improved my understanding of local account administration in Windows.

Key lessons learned:

- Local user accounts can be managed through Local Users and Groups.
- Group membership determines user permissions.
- The Administrators group provides elevated privileges.
- Standard Users have limited permissions.
- Reviewing group memberships is an important security practice.
- Access control helps protect systems from unauthorized changes.

This lab strengthened my understanding of user administration and permission management in Windows environments.

---

# Real World Scenario

## Ticket LU-001

A new employee requires local administrator access.

### Investigation

1. Open Local Users and Groups.
2. Review existing users.
3. Review Administrators group membership.
4. Verify business justification.
5. Add or remove access as required.

### Findings

Current administrative access was reviewed successfully.

### Resolution

No changes were required during this investigation.

---

# Interview Questions

## What is the difference between a standard user and an administrator?

Administrators have elevated privileges and can make system-wide changes. Standard users have limited permissions.

---

## Why should administrator access be restricted?

To reduce security risks and prevent unauthorized system changes.

---

## How do you view local users?

Run:

lusrmgr.msc

---

## How do you identify users with administrator rights?

Review membership of the Administrators group.
