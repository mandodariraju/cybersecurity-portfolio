# Incident Handler's Journal

## Date: 16 June 2026

**Entry:** 1

### Description

This journal entry documents a ransomware incident that affected a healthcare clinic. The incident disrupted business operations and prevented employees from accessing critical patient records after attackers deployed ransomware through a phishing email campaign. This investigation occurred during the **Detection and Analysis** phase of the NIST Incident Response Lifecycle.

### Tool(s) Used

* Incident Handler's Journal
* Incident Documentation Process
* 5 W's Analysis Method

### The 5 W's

**Who:**
An organized group of cybercriminals targeted the healthcare clinic using phishing emails containing malicious attachments.

**What:**
A ransomware attack encrypted critical organizational files and displayed a ransom note demanding payment for a decryption key.

**When:**
The incident occurred on a Tuesday morning at approximately 9:00 a.m.

**Where:**
The attack affected the healthcare clinic's internal systems, network infrastructure, and patient data resources.

**Why:**
Employees downloaded a malicious attachment from a phishing email, allowing ransomware to execute and encrypt critical files.

### Additional Notes

This incident demonstrates the importance of employee security awareness training, email security controls, and maintaining reliable backups. Further investigation would be required to determine the extent of system compromise and any potential data exposure.

---

## Date: 17 June 2026

**Entry:** 2

### Description

This journal entry documents a phishing investigation involving a malicious email attachment. Analysis confirmed that the attachment hash matched a known malicious file. This activity occurred during the **Detection and Analysis** phase of the NIST Incident Response Lifecycle.

### Tool(s) Used

* VirusTotal
* Threat Intelligence Sources
* Alert Ticket Documentation

### The 5 W's

**Who:**
An unknown threat actor sent a phishing email impersonating a job applicant.

**What:**
A malicious executable attachment was delivered through email and identified as malware.

**When:**
The phishing alert was generated after the suspicious email was detected and reviewed.

**Where:**
The incident targeted the organization's email system and an employee mailbox.

**Why:**
The attacker attempted to deliver malware and potentially gain unauthorized access to company systems.

### Additional Notes

The alert was escalated because the attachment hash was confirmed malicious. Security teams should block the file hash and review affected systems for indicators of compromise.

---

## Date: 18 June 2026

**Entry:** 3

### Description

This journal entry documents the use of Wireshark to analyze network packets and understand network communication. Packet analysis supports threat detection and troubleshooting by providing visibility into network traffic patterns.

### Tool(s) Used

* Wireshark

### Tool Notes

* Captured and analyzed network packets.
* Examined source and destination IP addresses.
* Reviewed protocol information and packet details.
* Applied filters to locate specific traffic.
* Improved understanding of network communications.

### Additional Notes

Wireshark provides a graphical interface that simplifies packet analysis and troubleshooting. It is useful for investigating suspicious network activity and identifying communication patterns.

---

## Date: 19 June 2026

**Entry:** 4

### Description

This journal entry documents the use of Splunk for log analysis and security monitoring. Splunk enables analysts to search, filter, and investigate large volumes of security event data efficiently.

### Tool(s) Used

* Splunk Enterprise

### Tool Notes

* Performed searches using keywords and filters.
* Investigated security logs and events.
* Identified suspicious activities through log analysis.
* Used queries to narrow search results.
* Reviewed security-related event information.

### Additional Notes

Splunk is valuable for security monitoring, incident investigations, and threat hunting. Effective searching helps analysts quickly identify anomalies and potential security incidents.

---

# Reflections / Notes

### Were there any specific activities that were challenging for you? Why or why not?

The most challenging activities involved analyzing logs and interpreting packet captures because they required careful attention to detail. As I practiced using cybersecurity tools, my understanding improved and I became more confident in identifying relevant information.

### Has your understanding of incident detection and response changed since taking this course?

Yes. I now better understand the incident response process and the importance of documentation, investigation, containment, and recovery. I also learned how structured frameworks help security teams respond effectively to incidents.

### Was there a specific tool or concept that you enjoyed the most? Why?

I enjoyed using Wireshark the most because it allowed me to see real network traffic and understand how devices communicate. It provided practical experience that strengthened my knowledge of network security and packet analysis.
