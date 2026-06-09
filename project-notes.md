## Admin Setup

### Group Created

Admins

### User Created

admin-user

### Policy Attached

AdministratorAccess

### MFA

Enabled on Root Account

### Verification

Successfully logged in using admin-user.



## Phase 2 - RBAC Design

Groups Created:

- Admins
- Developers
- DevOps
- Security
- Interns

Purpose:

Admins     -> Full administrative access
Developers -> Application development team
DevOps     -> Infrastructure team
Security   -> Audit and compliance team
Interns    -> Read-only access



## Phase 3 - Custom IAM Policies

Policies Created:

- developers-policy.json
- devops-policy.json
- security-policy.json
- interns-policy.json

Purpose:

Developers -> Limited application access
DevOps -> Infrastructure management
Security -> Audit and compliance access
Interns -> Read-only access



## Phase 4 - IAM Policies Created

Policies:

- DeveloperPolicy
- DevOpsPolicy
- SecurityPolicy
- InternPolicy

Created using custom JSON policies.

Stored locally in:
policies/




## Phase 5 - Users and Policy Assignment

Users Created:

- dev-user1
- devops-user1
- security-user1
- intern-user1

Group Assignments:

dev-user1 -> Developers
devops-user1 -> DevOps
security-user1 -> Security
intern-user1 -> Interns

Policies Attached:

Developers -> DeveloperPolicy
DevOps -> DevOpsPolicy
Security -> SecurityPolicy
Interns -> InternPolicy
