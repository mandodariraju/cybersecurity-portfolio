# Access Control Incident Investigation

## Scenario

A business reported a suspicious payroll transaction to an unknown bank account. Although the payment was stopped before completion, an investigation was conducted to identify the cause and recommend security improvements.

## Objective

Analyze event log data, identify access control weaknesses, and recommend mitigations to reduce the risk of future incidents.

## Event Log Findings

| Field        | Value                           |
| ------------ | ------------------------------- |
| Event Type   | Information                     |
| Event Source | AdsmEmployeeService             |
| Event ID     | 1227                            |
| Date         | 10/03/2023                      |
| Time         | 8:29:57 AM                      |
| User         | Legal\Administrator             |
| Computer     | Up2-NoGud                       |
| IP Address   | 152.207.255.255                 |
| Description  | Payroll event added (FAUX_BANK) |

## Notes

1. A payroll event was created on 10/03/2023 at 8:29:57 AM.
2. The activity was performed using the Legal\Administrator account from device Up2-NoGud and IP address 152.207.255.255.

## Access Control Issues Identified

### Issue 1: Excessive Privileges

The Administrator account possessed sufficient permissions to modify payroll information. This created a risk if the account became compromised.

### Issue 2: Weak Account Management

The incident suggests that privileged accounts may not have been properly monitored, reviewed, or restricted according to business requirements.

## Recommendations

### 1. Apply the Principle of Least Privilege (PoLP)

Grant employees only the minimum permissions necessary to perform their job functions.

### 2. Implement Multi-Factor Authentication (MFA)

Require MFA for all privileged and financial system accounts to reduce the risk of unauthorized access.

### 3. Conduct Regular Access Reviews

Review user permissions periodically and remove unnecessary privileges.

### 4. Strengthen Offboarding Procedures

Immediately disable accounts and revoke access when employees leave the organization.

## Skills Demonstrated

* Access Control Analysis
* Authentication and Authorization Review
* Security Log Analysis
* Principle of Least Privilege (PoLP)
* Multi-Factor Authentication (MFA)
* Security Recommendations and Risk Mitigation

## Tools and Concepts

* Event Logs
* Access Controls
* Authentication
* Authorization
* Accounting and Auditing
* Identity and Access Management (IAM)

## Outcome

Identified weaknesses in access control practices that could enable unauthorized payroll modifications and recommended security controls to improve authentication, authorization, and accountability.
