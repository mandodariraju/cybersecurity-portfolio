# DoS Incident Report Analysis

## Summary

The company experienced a security incident when network services became unavailable due to a flood of incoming ICMP packets. Investigation revealed that the disruption was caused by a Denial of Service (DoS) attack that exploited an improperly configured firewall. The cybersecurity team responded by blocking incoming ICMP traffic, stopping non-critical services, and restoring critical network operations.

## Identify

A malicious actor launched an ICMP flood attack against the company's network. The attack overwhelmed internal network resources and disrupted access to critical services. The primary vulnerability was an unconfigured firewall that allowed excessive ICMP traffic into the network.

## Protect

The cybersecurity team implemented new firewall rules to limit incoming ICMP traffic and deployed an IDS/IPS solution to filter suspicious packets. Regular firewall reviews, security audits, and network security policies should also be maintained to reduce future risks.

## Detect

Source IP address verification was enabled on the firewall to identify spoofed IP addresses. Network monitoring software and IDS/IPS tools were implemented to detect abnormal traffic patterns and provide early warning of potential attacks.

## Respond

For future incidents, the security team will isolate affected systems, block malicious traffic, analyze firewall and network logs, and restore critical services as quickly as possible. Incident details will be documented and reported to management, and response procedures will be reviewed after each event.

## Recover

Critical network services should be restored first, followed by non-critical services after network stability is confirmed. Firewall configurations should be reviewed and monitored continuously. Recovery procedures should be documented to improve the organization's ability to respond to future DoS attacks.

## Reflections/Notes

This activity demonstrated how the NIST Cybersecurity Framework can be used to analyze security incidents and improve organizational security. Proper firewall configuration, continuous monitoring, and IDS/IPS technologies are essential for defending against network-based attacks such as DoS and DDoS incidents.

