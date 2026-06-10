# AWS IAM Security Project

## Overview

This project demonstrates the implementation of Role-Based Access Control (RBAC) in AWS Identity and Access Management (IAM) using custom IAM policies, IAM groups, users, and permission validation.

The objective was to design a secure AWS account structure following the Principle of Least Privilege while validating access controls through real-world testing.

---

## Architecture

AWS Account
│
├── Admins
│ └── admin-user
│ └── AdministratorAccess
│
├── Developers
│ └── dev-user1
│ └── DeveloperPolicy
│
├── DevOps
│ └── devops-user1
│ └── DevOpsPolicy
│
├── Security
│ └── security-user1
│ └── SecurityPolicy
│
└── Interns
└── intern-user1
└── InternPolicy

---

## Technologies Used

- AWS IAM
- AWS EC2
- AWS S3
- AWS CloudWatch
- Git
- GitHub
- Linux (WSL Ubuntu)

---

## IAM Groups Created

- Admins
- Developers
- DevOps
- Security
- Interns

---

## IAM Users Created

- admin-user
- dev-user1
- devops-user1
- security-user1
- intern-user1

---

## Custom Policies

### DeveloperPolicy

Permissions:

- View EC2
- Start EC2
- Stop EC2
- Access S3
- Access CloudWatch

Restrictions:

- Cannot terminate EC2 instances

### DevOpsPolicy

Permissions:

- Manage EC2
- Manage S3
- Access CloudWatch

### SecurityPolicy

Permissions:

- View IAM
- View CloudTrail
- Perform audits

Restrictions:

- Cannot create infrastructure resources

### InternPolicy

Permissions:

- Read-only access

Restrictions:

- Cannot modify resources

---

## Security Features Implemented

- Role-Based Access Control (RBAC)
- Principle of Least Privilege
- IAM Groups
- Custom IAM Policies
- Permission Validation Testing
- MFA Enabled

---

## Permission Validation Results

### Developer
# AWS IAM Security Project

## Overview

This project demonstrates the implementation of Role-Based Access Control (RBAC) in AWS Identity and Access Management (IAM) using custom IAM policies, IAM groups, users, and permission validation.

The objective was to design a secure AWS account structure following the Principle of Least Privilege while validating access controls through real-world testing.

---

## Architecture

AWS Account
│
├── Admins
│ └── admin-user
│ └── AdministratorAccess
│
├── Developers
│ └── dev-user1
│ └── DeveloperPolicy
│
├── DevOps
│ └── devops-user1
│ └── DevOpsPolicy
│
├── Security
│ └── security-user1
│ └── SecurityPolicy
│
└── Interns
└── intern-user1
└── InternPolicy

---

## Technologies Used

- AWS IAM
- AWS EC2
- AWS S3
- AWS CloudWatch
- Git
- GitHub
- Linux (WSL Ubuntu)

---

## IAM Groups Created

- Admins
- Developers
- DevOps
- Security
- Interns

---

## IAM Users Created

- admin-user
- dev-user1
- devops-user1
- security-user1
- intern-user1

---

## Custom Policies

### DeveloperPolicy

Permissions:

- View EC2
- Start EC2
- Stop EC2
- Access S3
- Access CloudWatch

Restrictions:

- Cannot terminate EC2 instances

### DevOpsPolicy

Permissions:

- Manage EC2
- Manage S3
- Access CloudWatch

### SecurityPolicy

Permissions:

- View IAM
- View CloudTrail
- Perform audits

Restrictions:

- Cannot create infrastructure resources

### InternPolicy

Permissions:

- Read-only access

Restrictions:

- Cannot modify resources

---

## Security Features Implemented

- Role-Based Access Control (RBAC)
- Principle of Least Privilege
- IAM Groups
- Custom IAM Policies
- Permission Validation Testing
- MFA Enabled

---

## Permission Validation Results

### Developer

- View EC2: PASS
- Start EC2: PASS
- Stop EC2: PASS
- Terminate EC2: DENIED

### DevOps

- Manage EC2: PASS
- Manage S3: PASS

### Security

- View IAM: PASS
- Launch EC2: DENIED

### Intern

- View EC2: PASS
- Launch EC2: DENIED

---

## Project Outcomes

- Implemented secure AWS IAM architecture
- Designed custom least-privilege policies
- Validated permissions through real-world testing
- Documented architecture and security controls
- Maintained project using Git and GitHub

---

## Author

Harikrishna P V
- View EC2: PASS
- Start EC2: PASS
- Stop EC2: PASS
- Terminate EC2: DENIED

### DevOps

- Manage EC2: PASS
- Manage S3: PASS

### Security

- View IAM: PASS
- Launch EC2: DENIED

### Intern

- View EC2: PASS
- Launch EC2: DENIED

---

## Project Outcomes

- Implemented secure AWS IAM architecture
- Designed custom least-privilege policies
- Validated permissions through real-world testing
- Documented architecture and security controls
- Maintained project using Git and GitHub

---

## Author

Harikrishna P V
