# Bank Risk Register Analysis

## Project Description

This project involved analyzing risks affecting a banking organization and prioritizing them based on likelihood and severity. A risk register was used to identify potential threats, assess their impact on business operations, and determine which risks should be addressed first.

## Operational Environment

The bank operates in a coastal area with low crime rates and serves approximately 2,000 individual customers and 200 commercial customers. The organization employs 100 on-site employees and 20 remote employees. Due to strict financial regulations, protecting customer data and financial assets is critical.

## Risk Assessment

| Asset             | Risk                      | Likelihood | Severity | Priority |
| ----------------- | ------------------------- | ---------- | -------- | -------- |
| Funds             | Business Email Compromise | 2          | 2        | 4        |
| Customer Database | Compromised User Database | 2          | 3        | 6        |
| Financial Records | Data Leak                 | 3          | 3        | 9        |
| Safe              | Theft                     | 1          | 3        | 3        |
| Supply Chain      | Natural Disaster Delays   | 1          | 2        | 2        |

## Highest Priority Risk

The highest-priority risk identified was a financial records leak with a risk score of 9. The risk exists because a backup database server is publicly accessible. If exploited, sensitive financial data could be exposed, resulting in regulatory penalties, reputational damage, and operational disruption.

## Recommendations

* Secure database backups and restrict public access.
* Implement strong encryption for customer data.
* Conduct regular security audits.
* Provide phishing awareness training to employees.
* Enforce access controls and least-privilege principles.
* Monitor third-party and supply-chain risks.

## Summary

This activity demonstrated how organizations identify, evaluate, and prioritize cybersecurity risks. By assessing both likelihood and severity, security teams can focus resources on the most critical threats and improve the organization's overall security posture.
