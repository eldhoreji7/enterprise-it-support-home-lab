# Scenario 02 – Entra ID Account Disable and Session Revocation

## Scenario

A simulated employee account needed to be immediately blocked as part of an offboarding or security response process.

## Environment

- Microsoft Entra ID
- Microsoft Entra ID Free tenant
- Test user: John Smith
- Department: Sales
- Role: Sales Coordinator

## Actions Performed

1. Located John Smith in Microsoft Entra ID.
2. Opened the user's account overview.
3. Changed the account status from Enabled to Disabled.
4. Attempted a new sign-in using the disabled account.
5. Confirmed that the user could no longer authenticate.
6. Reviewed Entra ID sign-in logs for the blocked sign-in attempt.
7. Revoked the user's existing sign-in sessions.
8. Verified that session revocation completed successfully.
9. Re-enabled the account after completing the lab exercise.

## Why Both Actions Matter

Disabling an account prevents new authentication attempts.

Revoking sessions invalidates existing authentication sessions and forces the user to authenticate again.

Using both controls is useful during:

- Employee offboarding
- Suspected account compromise
- Lost or stolen devices
- Security incidents

## Skills Demonstrated

- Microsoft Entra ID administration
- User lifecycle management
- Account disable and enable procedures
- Session revocation
- Authentication troubleshooting
- Sign-in log investigation
- Security incident response
- Offboarding procedures

## Security Notes

- All activities were performed using simulated lab accounts.
- No production identities were used.
- Credentials and sensitive identifiers were excluded from documentation.

## Outcome

The user's account was successfully blocked from signing in and existing sessions were revoked. The account was later restored for continued lab testing.
