# Phishing Incident Response

## Overview

This activity involved investigating a phishing alert as a Level 1 Security Operations Center (SOC) analyst. The objective was to analyze a suspicious email, validate the attachment's reputation using threat intelligence, follow the phishing response playbook, and determine the appropriate response action.

## Alert Details

**Alert ID:** A-2703

**Severity:** Medium

**Alert Type:** Possible phishing attempt involving malware delivery

**Known Malicious SHA256 Hash:**

54e6ea47eb04634d3e87fd7787e2136ccfbcc80ade34f246a12cf93bab527f6b

## Investigation

The email claimed to be from a job applicant applying for an Infrastructure Engineer position. Several indicators suggested the message was malicious:

* Suspicious sender email address and IP address
* Multiple spelling and grammar errors
* Password-protected attachment designed to bypass email scanning
* Executable attachment named `bfsvc.exe`
* Attachment hash previously verified as malicious

## Playbook Actions Performed

1. Reviewed alert severity and ticket details.
2. Examined sender, recipient, subject line, and message body.
3. Identified the presence of a file attachment.
4. Verified the attachment hash as malicious using threat intelligence information.
5. Followed the phishing response playbook.
6. Escalated the incident to a Level 2 SOC analyst.

## Ticket Resolution

**Status:** Escalated

### Reason for Escalation

The email contained a malicious executable attachment whose SHA256 hash had already been confirmed as malicious. The sender information appeared suspicious, and the use of a password-protected attachment indicated an attempt to evade security controls. Based on the phishing playbook procedures, escalation was required for further containment and remediation.

## Skills Demonstrated

* Phishing Analysis
* Alert Triage
* Incident Response
* Threat Intelligence
* Malware Identification
* Security Playbook Usage
* SOC Operations
* SHA256 Hash Analysis
