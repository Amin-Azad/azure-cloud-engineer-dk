# Part 1 — Entra ID Users Setup

## Objective
Prepare 3 Azure test identities for RBAC testing.

## Users Created

| Display Name | Username | Purpose |
|---|---|---|
| Test Owner | owner1@[yourdomain].onmicrosoft.com | Will receive Owner role in Part 2 |
| Test Contributor | contributor1@[yourdomain].onmicrosoft.com | Will receive Contributor role in Part 2 |
| Test Reader | reader1@[yourdomain].onmicrosoft.com | Will receive Reader role in Part 2 |

## Notes
- All users were created using Azure Portal.
- Temporary passwords were generated and stored securely.
- These accounts will be used for RBAC testing in Part 2.

## Key Concepts Learned
- Microsoft Entra ID is Azure’s identity platform.
- Member users are internal tenant users.
- Guest users are for external access.
- Security groups are used for RBAC
