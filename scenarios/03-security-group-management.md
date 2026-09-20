# Scenario 03 – Entra ID Security Group Management

## Scenario

A Sales employee required membership in a departmental security group so that access could be managed through group-based administration rather than individual assignments.

## Environment

- Microsoft Entra ID
- Security group: SG-Sales-Users
- Test user: John Smith
- Department: Sales
- Delegated administrator: Helpdesk Technician

## Actions Performed

1. Created an Entra ID security group named `SG-Sales-Users`.
2. Used an Assigned membership model.
3. Assigned the Helpdesk Technician the `Groups Administrator` directory role.
4. Signed in using the delegated Helpdesk Technician account.
5. Verified the security group in Microsoft Entra ID.
6. Added John Smith as a member of the Sales security group.
7. Verified that John Smith appeared in the group membership list.

## Why Group-Based Access Matters

Security groups allow administrators to manage access for multiple users through group membership instead of assigning permissions individually.

This helps provide:

- Consistent access control
- Easier onboarding and offboarding
- Reduced administrative effort
- Better scalability
- Least-privilege access management

## Skills Demonstrated

- Microsoft Entra ID group administration
- Security group management
- Delegated administration
- Groups Administrator role
- Least privilege
- User access management
- Enterprise naming conventions

## Outcome

John Smith was successfully added to the `SG-Sales-Users` security group using a delegated administrator account.
