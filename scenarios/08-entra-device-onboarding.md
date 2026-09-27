# Scenario 08 – Microsoft Entra ID Device Onboarding

## Scenario
A new employee, John Smith, required a company workstation to be joined to Microsoft Entra ID and configured for organisational sign-in.

## Lab Environment
- Windows 11 Pro (UTM virtual machine)
- Microsoft Entra ID
- Local administrator: LabAdmin
- Employee: John Smith
- Workstation: WIN-MFK0K8QP286

## Implementation
1. Verified the Windows edition using winver.
2. Checked the initial device registration state using dsregcmd /status.
3. Opened Settings > Accounts > Access work or school.
4. Selected Join this device to Microsoft Entra ID.
5. Authenticated using John Smith's organisational account.
6. Successfully connected the workstation to the Entra tenant.
7. Verified the device appeared in the Entra device inventory with join type Microsoft Entra joined.
8. Completed John's first organisational Windows sign-in.
9. Verified the session identity using whoami.
10. Reviewed local Administrators group membership.
11. Checked the user's security token using whoami /groups.

## Verification
- Device registration: Successful
- Device join type: Microsoft Entra joined
- Employee identity: azuread\johnsmith
- Local Windows profile: C:\Users\johnsmith
- Local administrator membership: Administrator and LabAdmin
- John Smith: Standard user

## Skills Demonstrated
- Windows 11 device onboarding
- Microsoft Entra device joining
- Organisational account sign-in
- Windows user profile provisioning
- Device inventory verification
- Windows account and group troubleshooting
- Least-privilege verification

## Outcome
Successfully onboarded a Windows 11 workstation into Microsoft Entra ID and verified the employee's organisational sign-in and standard-user permissions.
