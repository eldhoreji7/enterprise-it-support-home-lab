# Enterprise IT Support & Microsoft 365 Home Lab

A hands-on IT support lab designed to simulate real-world Service Desk, Desktop Support, Microsoft Entra ID, Microsoft 365 and endpoint administration tasks.

The goal of this project is to demonstrate practical troubleshooting, identity administration, user lifecycle management and enterprise IT support skills using realistic support scenarios.

## Lab Environment

- MacBook Air M1
- UTM Virtualization
- Windows 11 ARM
- Microsoft Azure
- Microsoft Entra ID
- Microsoft 365
- Command Prompt / Windows Administration

## Skills Demonstrated

- Windows 11 administration
- TCP/IP and DNS troubleshooting
- Local user and group management
- Standard vs administrator permissions
- Microsoft Entra ID user administration
- Password reset and authentication troubleshooting
- Sign-in log investigation
- Account disable and enable procedures
- Session revocation
- User lifecycle management
- Security group management
- Service Desk incident documentation

## Support Scenarios

### 01 – Password Reset and Sign-In Verification

Simulated a user authentication issue, performed a password reset in Microsoft Entra ID, tested the temporary-password workflow and verified successful authentication using Entra sign-in logs.

[View Scenario 01](scenarios/01-password-reset-signin-verification.md)

### 02 – Account Disable and Session Revocation

Simulated an employee offboarding/security response by disabling an Entra ID account, testing blocked authentication, reviewing sign-in activity and revoking existing user sessions.

[View Scenario 02](scenarios/02-account-disable-session-revocation.md)

### 03 – Security Group Management

Created and managed the `SG-Sales-Users` security group in Microsoft Entra ID, used delegated administration through the Groups Administrator role, and verified John Smith's departmental group membership.

[View Scenario 03](scenarios/03-security-group-management.md)

## Project Status

### 04 — Delegated Helpdesk Password Reset

Practised delegated IT administration by using the Helpdesk Administrator role to reset a test user's password in Microsoft Entra ID.

[View Scenario 04](scenarios/04-delegated-helpdesk-password-reset.md)

### 05 — Group Access Removal and Restoration

Simulated troubleshooting user access by removing and restoring Microsoft Entra security group membership.

[View Scenario 05](scenarios/05-group-access-removal-restoration.md)

### 06 — Failed Sign-in Investigation

Investigated Microsoft Entra sign-in logs to identify authentication failures and document troubleshooting findings.

[View Scenario 06](scenarios/06-failed-signin-investigation.md)

### 07 — MFA Recovery Using Temporary Access Pass

Practised an account recovery workflow using Microsoft Entra authentication methods and Temporary Access Pass.

[View Scenario 07](scenarios/07-mfa-recovery-temporary-access-pass.md)

### 08 — Microsoft Entra Device Onboarding

Joined a Windows 11 virtual machine to Microsoft Entra ID and verified device registration and standard-user permissions.

[View Scenario 08](scenarios/08-entra-device-onboarding.md)

### 09 — Windows Network and DNS Troubleshooting

Performed Windows network diagnostics, including IP configuration checks, DNS resolution testing and troubleshooting a simulated DNS failure.

[View Scenario 09](scenarios/09-windows-network-dns-troubleshooting.md)

### 10 — Service Desk Ticket Management and Outlook Troubleshooting

Created a Microsoft Forms support request form and manual Excel ticket tracker. Tested Outlook DNS and HTTPS connectivity, documented troubleshooting findings and simulated escalation of an unresolved incident.

[View Scenario 10](scenarios/10-service-desk-ticket-management.md)


This project is actively being expanded with:

- Microsoft Entra ID security groups
- Microsoft 365 administration
- MFA and authentication methods
- Intune endpoint management
- Microsoft Forms and Power Automate
- SharePoint-based Service Desk ticketing
- Additional troubleshooting scenarios

## Security

All users, identities and scenarios in this repository are simulated lab accounts.

Passwords, credentials, tenant identifiers and unnecessary personal information are excluded from public documentation.
