# Scenario 01 – Entra ID Password Reset and Sign-In Verification

## Scenario

A simulated employee, John Smith from the Sales department, was unable to access his Microsoft account and required a password reset.

## Environment

- Microsoft Entra ID
- Microsoft Entra ID Free tenant
- Test user: John Smith
- Department: Sales
- Role: Sales Coordinator

## Troubleshooting and Resolution

1. Located the user account in Microsoft Entra ID.
2. Verified that the correct employee account was selected.
3. Reset the user's password from the Entra admin portal.
4. Generated a temporary password for the user.
5. Signed in using a private browser session to simulate the employee experience.
6. Completed the required password change during first sign-in.
7. Confirmed that the user could successfully access the Microsoft My Account portal.
8. Reviewed Entra ID sign-in logs to verify successful authentication.

## Verification

The Entra ID sign-in logs showed successful interactive sign-ins after the password reset and password-change process.

An earlier interrupted sign-in was also observed during the temporary-password workflow, demonstrating how authentication events can be investigated through Entra ID sign-in logs.

## Skills Demonstrated

- Microsoft Entra ID user administration
- Password reset procedures
- Identity and access troubleshooting
- Sign-in log analysis
- End-user support
- Service Desk incident resolution
- Verification and documentation

## Security Notes

- Temporary passwords were not stored in this repository.
- Credentials and sensitive identifiers are excluded from screenshots.
- Test accounts were used for all lab activities.

## Outcome

The user's access was successfully restored and verified through both the end-user sign-in process and Entra ID sign-in logs.
