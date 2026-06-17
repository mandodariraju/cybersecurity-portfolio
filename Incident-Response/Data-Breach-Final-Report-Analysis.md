# Data Breach Final Report Analysis

## Overview

This project reviews a completed incident final report involving a data breach that exposed customer personally identifiable information (PII) and financial data. The objective was to understand the incident lifecycle, identify the root cause, review response actions, and evaluate recommendations for preventing similar incidents.

## Incident Summary

On December 28, 2022, an attacker gained unauthorized access to customer data through a vulnerability in the company's e-commerce web application. Approximately 50,000 customer records containing personal and financial information were exposed.

The estimated financial impact of the incident was approximately $100,000 in direct costs and potential revenue loss.

## Timeline

### December 22, 2022

* An employee received an email claiming customer data had been stolen.
* The sender demanded a cryptocurrency payment.
* The email was mistakenly treated as spam and deleted.

### December 28, 2022

* The attacker sent a second email containing samples of stolen customer data.
* The payment demand increased.
* The security team was notified and initiated an investigation.

### December 28–31, 2022

* Security personnel investigated the incident.
* Web application logs were analyzed.
* The root cause was identified and remediation efforts began.

## Root Cause Analysis

The investigation determined that the breach resulted from a forced browsing vulnerability in the e-commerce application.

The attacker manipulated order numbers contained within URL parameters to access purchase confirmation pages belonging to other customers. This allowed unauthorized access to sensitive customer information and enabled large-scale data collection.

## Response Actions

The organization performed the following actions:

* Investigated web application access logs
* Identified abnormal sequential requests to customer order pages
* Confirmed unauthorized access activity
* Notified affected customers
* Coordinated public disclosure efforts
* Offered identity protection services to impacted customers

## Security Recommendations

To reduce future risk, the report recommended:

1. Conduct regular vulnerability assessments and penetration testing.
2. Implement URL allowlisting controls.
3. Restrict access to authorized and authenticated users only.
4. Improve monitoring and logging of web application activity.
5. Strengthen access control mechanisms for sensitive customer data.

## Skills Demonstrated

* Incident Response
* Data Breach Investigation
* Root Cause Analysis
* Log Analysis
* Web Application Security
* Vulnerability Assessment
* Security Reporting
* Risk Mitigation Planning
* Access Control Concepts
