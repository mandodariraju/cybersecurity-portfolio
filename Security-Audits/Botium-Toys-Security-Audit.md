# Botium Toys Security Audit

## Overview

Conducted an internal security audit of Botium Toys based on the NIST Cybersecurity Framework (CSF). The objective was to identify missing security controls, assess compliance requirements, and recommend improvements.

## Key Findings

* Least privilege not implemented
* Separation of duties not implemented
* No disaster recovery plan
* No backups of critical data
* No encryption for customer payment information
* No intrusion detection system (IDS)
* Weak password policy and no centralized password management
* Firewall and antivirus are implemented
* Physical security controls such as locks, CCTV, and fire prevention systems are in place

## Compliance Review

### PCI DSS

* Not fully compliant due to lack of encryption and access restrictions.

### GDPR

* 72-hour breach notification process exists.
* Data classification and protection need improvement.

### SOC

* Data integrity controls exist.
* User access controls require improvement.

## Recommendations

Implement least privilege, separation of duties, encryption, IDS, regular backups, stronger password policies, centralized password management, and a disaster recovery plan.
