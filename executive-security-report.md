# Northstar Financial Group
# IAM Access Review Security Assessment

## Executive Summary

A security-focused Identity and Access Management (IAM) review was conducted within the Microsoft Entra ID environment for Northstar Financial Group.

The assessment focused on:
- User access governance
- Administrative privilege review
- Stale account identification
- Identity lifecycle management
- Authentication security controls
- Audit and sign-in log analysis

Multiple IAM security risks were identified, including excessive administrative privileges and inactive account exposure. Remediation activities were performed to reduce organizational risk and improve least privilege alignment.

## Security Findings

| Finding | Risk Level | Status |
|---|---|---|
| Overprivileged IT support account | High | Partially Remediated |
| Stale contractor account | Medium | Remediated |
| Lack of MFA enforcement prior to hardening review | Medium | Improved |
| Identity lifecycle management gaps | Medium | Improved |

## Detailed Findings

### 1. Excessive Administrative Privileges

An IT support account was assigned Global Administrator access beyond operational necessity.

Risk:
- Full tenant compromise potential
- Excessive privilege exposure
- Increased attack surface

Remediation:
- Remediation attempted and documented
- Tenant role removal limitations encountered within Entra ID Free environment
- Escalation path documented

---

### 2. Stale Contractor Account

A contractor account remained active without valid business justification.

Risk:
- Unauthorized persistent access
- Increased identity attack surface

Remediation:
- Account sign-in blocked successfully

---

### 3. Identity Lifecycle Risks

User lifecycle workflows initially lacked formalized onboarding/offboarding controls.

Risk:
- Privilege creep
- Orphaned access
- Improper access retention

Remediation:
- Simulated Joiner/Mover/Leaver lifecycle process implemented


## Security Recommendations

Recommended future improvements:
- Implement Conditional Access policies
- Enforce MFA for all privileged accounts
- Conduct recurring quarterly access reviews
- Implement Privileged Identity Management (PIM)
- Automate stale account detection
- Integrate Entra logs into a SIEM platform
- Apply Zero Trust identity principles

## Analyst Summary

This project demonstrated practical IAM and cloud identity security operations using Microsoft Entra ID.

Skills demonstrated:
- User and group provisioning
- RBAC administration
- Administrative privilege analysis
- Access review methodology
- IAM remediation workflows
- Audit log investigation
- Sign-in monitoring
- Identity lifecycle management
- MFA/security hardening concepts
- Security documentation and reporting

This lab simulated realistic IAM analyst responsibilities commonly performed in enterprise cloud environments.