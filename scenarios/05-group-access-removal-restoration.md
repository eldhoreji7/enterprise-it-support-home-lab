# Scenario 05 – Group Access Removal and Restoration

## Scenario

A simulated employee had transferred out of the Sales department and required removal from the Sales security group.

The change was performed using a delegated Helpdesk Technician account rather than a Global Administrator account.

## Environment

- Microsoft Entra ID
- Security group: SG-Sales-Users
- Test user: John Smith
- Delegated administrator: Helpdesk Technician
- Role: Groups Administrator

## Actions Performed

1. Signed into Microsoft Entra using the Helpdesk Technician account.
2. Opened the `SG-Sales-Users` security group.
3. Verified that John Smith was a direct member.
4. Removed John Smith from the security group.
5. Verified that the membership was removed.
6. Reviewed the group's Microsoft Entra audit logs.
7. Located the `Remove member from group` event.
8. Confirmed the event completed successfully.
9. Verified that the initiating account was the Helpdesk Technician.
10. Added John Smith back to the group after completing the test.

## Why This Matters

Group membership is commonly used to control access to applications, resources and departmental services.

Removing users from groups is an important part of:

- Department transfers
- Access reviews
- Offboarding
- Least-privilege administration
- Security incident response

## Skills Demonstrated

- Microsoft Entra ID security group management
- Delegated administration
- Groups Administrator role
- User access removal
- Audit log investigation
- Least privilege
- Access lifecycle management
- Service Desk change verification

## Outcome

John Smith was successfully removed from the Sales security group by the delegated Helpdesk Technician account.

The action was verified in Microsoft Entra audit logs and the user was later restored to the group for continued lab testing.
