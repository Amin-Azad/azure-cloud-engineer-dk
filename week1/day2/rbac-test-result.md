# RBAC Live Test Results — Day 2

## Resource Group
day2-rg (northeurope)

## Users and Roles

| User | Role |
|------|------|
| owner1 | Owner |
| contributor1 | Contributor |
| reader1 | Reader |

## Test Results

| Action | owner1 | contributor1 | reader1 |
|--------|--------|--------------|----------|
| View resources | ✓ | ✓ | ✓ |
| Create resources | ✓ | ✓ | ✗ |
| Delete resources | ✓ | ✓ | ✗ |
| Assign roles | ✓ | ✗ | ✗ |

## Key Finding

RBAC is additive:
After assigning Contributor to reader1,
they could create resources.

## Conclusion

- Owner = full control
- Contributor = manage resources, no access control
- Reader = view only
