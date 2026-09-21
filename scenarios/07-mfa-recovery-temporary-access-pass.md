# Scenario 07 – Lost MFA Method Recovery Using Temporary Access Pass

## Scenario

A simulated employee lost access to their registered Microsoft Authenticator method and could no longer complete normal MFA verification.

The issue was recovered using delegated Microsoft Entra administration and a Temporary Access Pass.

## Environment

- Microsoft Entra ID
- Test user: John Smith
- Support account: Helpdesk Technician
- Authentication method: Microsoft Authenticator
- Recovery method: Temporary Access Pass
- Delegated role: Authentication Administrator

## Troubleshooting and Recovery

1. Opened John Smith's Authentication methods in Microsoft Entra ID.
2. Verified the existing Microsoft Authenticator and passkey configuration.
3. Required the user to re-register multifactor authentication.
4. Confirmed that the previous Microsoft Authenticator registration was removed.
5. Attempted user verification with the remaining passkey.
6. Determined that the user's device no longer contained the matching passkey.
7. Created a one-time Temporary Access Pass for account recovery.
8. Signed in to the Security info portal using the Temporary Access Pass.
9. Registered Microsoft Authenticator again on the user's device.
10. Completed the Authenticator verification process.
11. Verified the newly registered Microsoft Authenticator from the administrator portal.
12. Confirmed that the Temporary Access Pass had been used.
13. Deleted the used Temporary Access Pass.
14. Verified that Microsoft Authenticator was the user's preferred MFA method.

## Least-Privilege Approach

The recovery was performed using the delegated Helpdesk Technician account with the Authentication Administrator role rather than Global Administrator privileges.

Temporary Access Pass was used as a short-lived recovery credential and removed after successful MFA registration.

## Skills Demonstrated

- Microsoft Entra ID authentication administration
- MFA troubleshooting
- Microsoft Authenticator recovery
- Temporary Access Pass
- Authentication Administrator role
- Delegated administration
- Least privilege
- Identity recovery
- Security information management
- Post-resolution verification

## Outcome

John Smith successfully regained access to Microsoft Authenticator using a Temporary Access Pass.

The temporary recovery credential was removed after use, and Microsoft Authenticator was restored as the user's usable and preferred MFA method.
