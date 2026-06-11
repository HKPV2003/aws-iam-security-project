# AWS IAM Security Project

## Overview

This project demonstrates the implementation of Role-Based Access Control (RBAC) in AWS Identity and Access Management (IAM) using custom IAM policies, IAM groups, users, and permission validation testing.

The objective was to design a secure AWS account structure following the Principle of Least Privilege while validating access controls through real-world testing scenarios.

---

## Architecture

```text
AWS Account
│
├── Admins
│   └── admin-user
│       └── AdministratorAccess
│
├── Developers
│   └── dev-user1
│       └── DeveloperPolicy
│
├── DevOps
│   └── devops-user1
│       └── DevOpsPolicy
│
├── Security
│   └── security-user1
│       └── SecurityPolicy
│
└── Interns
    └── intern-user1
        └── InternPolicy
```

---

## Technologies Used

* AWS IAM
* AWS EC2
* AWS S3
* AWS CloudWatch
* Git
* GitHub
* Linux (WSL Ubuntu)

---

## IAM Groups Created

* Admins
* Developers
* DevOps
* Security
* Interns

---

## IAM Users Created

* admin-user
* dev-user1
* devops-user1
* security-user1
* intern-user1

---

## Custom Policies

### DeveloperPolicy

**Permissions**

* View EC2 resources
* Start EC2 instances
* Stop EC2 instances
* Access S3 buckets
* Access CloudWatch

**Restrictions**

* Cannot terminate EC2 instances

---

### DevOpsPolicy

**Permissions**

* Manage EC2 resources
* Manage S3 resources
* Access CloudWatch

---

### SecurityPolicy

**Permissions**

* View IAM resources
* View CloudTrail logs
* Perform security audits

**Restrictions**

* Cannot create infrastructure resources

---

### InternPolicy

**Permissions**

* Read-only access to resources

**Restrictions**

* Cannot create, modify, or delete resources

---

## Security Features Implemented

* Role-Based Access Control (RBAC)
* Principle of Least Privilege
* IAM Groups
* Custom IAM Policies
* Multi-Factor Authentication (MFA)
* Permission Validation Testing

---

## Permission Validation Results

### Developer

* View EC2: PASS
* Start EC2: PASS
* Stop EC2: PASS
* Terminate EC2: DENIED

### DevOps

* Manage EC2: PASS
* Manage S3: PASS

### Security

* View IAM: PASS
* Launch EC2: DENIED

### Intern

* View EC2: PASS
* Launch EC2: DENIED

---

## Project Screenshots

The `screenshots/` folder contains evidence of:

* IAM Group Creation
* IAM User Creation
* Custom Policy Creation
* Policy Attachments
* RBAC Design
* Permission Validation Testing
* Architecture Documentation

---

## Project Duration

Completed in 3 days.

---

## Key Learning Outcomes

* AWS IAM Administration
* RBAC Implementation
* Principle of Least Privilege
* IAM Policy Design
* Security Best Practices
* Permission Validation Testing
* MFA Configuration
* Git & GitHub Documentation

---

## Project Outcomes

* Implemented secure AWS IAM architecture
* Designed custom least-privilege policies
* Validated permissions through real-world testing
* Documented architecture and security controls
* Maintained project using Git and GitHub
* Improved understanding of AWS security fundamentals

---

## Repository Structure

```text
aws-iam-security-project
├── architecture/
├── policies/
├── screenshots/
├── testing/
├── README.md
├── project-notes.md
└── project-summary.md
```

---

## Author

**Harikrishna P V**

Cloud & DevOps Learner | AWS | Linux | Docker | GitHub

