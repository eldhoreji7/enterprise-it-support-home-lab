# Scenario 06 – Failed Sign-In Investigation

## Scenario

A simulated employee reported that they were unable to sign in to their Microsoft account.

The issue was investigated using Microsoft Entra ID sign-in logs before making any changes to the user's account.

## Environment

- Microsoft Entra ID
- Test user: John Smith
- Support account: Helpdesk Technician
- Role: Reports Reader

## Troubleshooting Process

1. Reproduced a failed sign-in attempt using the John Smith test account.
2. Signed into Microsoft Entra using the Helpdesk Technician account.
3. Opened John Smith's sign-in logs.
4. Located the most recent failed interactive sign-in.
5. Reviewed the sign-in error information and authentication details.
6. Determined that the failure was caused by incorrect credentials.
7. Verified that the account itself was still enabled and healthy.
8. Had the user retry using the correct password.
9. Confirmed a successful sign-in afterward.
10. Verified the successful authentication in Entra ID sign-in logs.

## Troubleshooting Approach

The password was not reset because the sign-in logs showed that the account itself was healthy and the failure was caused by incorrect credentials.

This avoided making an unnecessary account change.

## Skills Demonstrated

- Microsoft Entra ID sign-in log investigation
- Authentication troubleshooting
- Root-cause analysis
- Reports Reader role
- Service Desk troubleshooting
- End-user support
- Verification after resolution
- Avoiding unnecessary administrative changes

## Outcome

The sign-in issue was diagnosed as an incorrect-password attempt.

The user successfully signed in with the correct credentials, and the successful authentication was verified through Microsoft Entra ID sign-in logs.
