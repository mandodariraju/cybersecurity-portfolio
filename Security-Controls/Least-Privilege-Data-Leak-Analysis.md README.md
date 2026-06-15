# Least Privilege Data Leak Analysis

## Incident Summary

A sales manager shared access to an internal folder containing confidential company information, including unreleased product details, customer analytics, and promotional materials. Access permissions were not revoked after the meeting. Later, a sales representative accidentally shared the internal folder link with a business partner, who publicly posted the link on social media, resulting in a data leak.

## Issue(s)

Several factors contributed to the information leak:

- Excessive access permissions were granted to employees.
- Access to the internal folder was not revoked after the meeting.
- Sensitive and public materials were stored together.
- Employees had access to information beyond what was required for their role.
- Human error resulted in accidental sharing of confidential information.

## Review

NIST SP 800-53 AC-6 (Least Privilege) states that users should only receive the minimum level of access necessary to perform their job responsibilities.

The control recommends:

- Restricting access based on job roles
- Automatically revoking temporary access
- Maintaining activity logs
- Regularly auditing user permissions

## Recommendations

- Implement Role-Based Access Control (RBAC).
- Restrict access to confidential product information.
- Separate internal documents from promotional materials.
- Configure temporary permissions to expire automatically.
- Conduct periodic access reviews and audits.
- Provide employee training on secure information sharing.

## Justification

Applying the principle of least privilege reduces the risk of unauthorized access and accidental disclosure of sensitive information. Limiting access based on job responsibilities decreases the number of users who can access confidential data. Regular audits and automatic permission expiration help maintain appropriate access levels while reducing security risks.

## Skills Demonstrated

- Access Control Management
- Least Privilege Principle
- Data Leak Prevention
- Security Policy Analysis
- NIST SP 800-53
- Security Recommendations
