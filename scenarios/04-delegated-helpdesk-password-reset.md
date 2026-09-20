# Scenario 04 – Delegated Helpdesk Password Reset

## Scenario

A user required a password reset, but the support task needed to be completed using a delegated Helpdesk Technician account rather than a Global Administrator account.

## Environment

- Microsoft Entra ID
- Test user: John Smith
- Support account: Helpdesk Technician
- Delegated role: Helpdesk Administrator
- Reporting role: Reports Reader

## Actions Performed

1. Assigned the Helpdesk Technician the Helpdesk Administrator role.
2. Signed into Microsoft Entra using the delegated support account.
3. Located John Smith's user account.
4. Reset the user's password.
5. Generated a temporary password for the user.
6. Opened the user's Entra audit logs.
7. Used Reports Reader permissions to review the audit event.
8. Verified the `Reset password (by admin)` activity.
9. Confirmed the action completed successfully.
10. Verified that the initiating account was the Helpdesk Technician.

## Least-Privilege Approach

The password reset was performed without giving the Helpdesk Technician Global Administrator privileges.

The support account was given only the permissions required for its responsibilities:

- Helpdesk Administrator – password and user support tasks
- Groups Administrator – security group administration
- Reports Reader – audit and sign-in log visibility

## Skills Demonstrated

- Delegated Microsoft Entra administration
- Password reset procedures
- Role-based access control
- Least privilege
- Audit log investigation
- User support
- Identity troubleshooting
- Administrative verification

## Outcome

John Smith's password was successfully reset by the delegated Helpdesk Technician account, and the action was verified through Microsoft Entra audit logs.
