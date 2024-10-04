# NIST-CSF-Security-Incident-Report

1. [Introduction](#introduction)
2. [Scenario](#scenario)
3. [Objective](#objective)
4. [Incident Report Analysis](#incident_report_analysis)
5. [Notes](#notes)
6. [Reflections](#reflections) 


# Introduction <a name="introduction"> 
A mock security incident report done as part of Cybersecurity documentation portfolio and Google's Coursera Cybersecurity Certificate as part of the [Connect and Protect: Networks and Network Security course] to gain an understanding of network-level vulnerabilities and how to secure networks.

# Scenario <a name="scenario"> 
You are a cybersecurity analyst working for a multimedia company that offers web design services, graphic design, and social media marketing solutions to small businesses. Your organization recently experienced a DDoS attack, which compromised the internal network for two hours until it was resolved.

During the attack, your organization’s network services suddenly stopped responding due to an incoming flood of ICMP packets. Normal internal network traffic could not access any network resources. The incident management team responded by blocking incoming ICMP packets, stopping all non-critical network services offline, and restoring critical network services. 

The company’s cybersecurity team then investigated the security event. They found that a malicious actor had sent a flood of ICMP pings into the company’s network through an unconfigured firewall. This vulnerability allowed the malicious attacker to overwhelm the company’s network through a distributed denial of service (DDoS) attack. 

To address this security event, the network security team implemented: 

- A new firewall rule to limit the rate of incoming ICMP packets

- Source IP address verification on the firewall to check for spoofed IP addresses on incoming ICMP packets

- Network monitoring software to detect abnormal traffic patterns

- An IDS/IPS system to filter out some ICMP traffic based on suspicious characteristics


# Objective  <a name="objective"> 
You are tasked with using this security event to create a plan to improve your company’s network security, following _the National Institute of Standards and Technology (NIST) Cybersecurity Framework (CSF_). 

The different steps of analyzing this cybersecurity incident and integrate your analysis into a general security strategy align with NIST's CSF's five core functions:

- **Identify** security risks through regular audits of internal networks, systems, devices, and access privileges to identify potential gaps in security. 

- **Protect** internal assets through the implementation of policies, procedures, training and tools that help mitigate cybersecurity threats. 

- **Detect** potential security incidents and improve monitoring capabilities to increase the speed and efficiency of detections. 

- **Respond** to contain, neutralize, and analyze security incidents; implement improvements to the security process. 

- **Recover** affected systems to normal operation and restore systems data and/or assets that have been affected by an incident.

# Incident Report Analysis <a name="incident_report_analysis"> 

## Summary
A security incident occcured where the organization’s internal network experienced a distributed denial of service (DDoS) attack. During the attack, the organization’s network services suddenly stopped responding. Devices on the internet network were affected and network resources within the affected network could not be accessed.

| Phase  | Description of what happened at each NIST CSF phase |
| --- | --- |
| Identify | The cybersecurity team investigated the security event and discovered a malicious actor exploited a vulnerability in the company's firewall to launch a Distributed Denial of Service (DDoS) attack. This attack involved sending a large number of Internet Control Message Protocol (ICMP) Ping requests to the network, overwhelming it and disrupting normal operations. The firewall was misconfigured, allowing the attacker to flood the network with traffic.   |
| Protect | The Cybersecurity team implemented two measures to prevent future DDoS attacks. Firewall rule: A new rule was added to the firewall to restrict the rate of incoming ICMP packets and. IDS/IPS system: An intrusion detection and prevention system was deployed to filter out suspicious ICMP traffic to the internal network. This system can identify and block malicious traffic based on its characteristics.  |
| Detect | Implement network monitoring software: This software will monitor network traffic for unusual patterns that may indicate a malicious activity or attack. Source IP address verification to configure the firewall will be configured to verify the source IP addresses of incoming ICMP packets. This will help identify spoofed IP addresses, which attackers often use to disguise their identity  |
| Respond | The incident management team took swift action to contain the DDoS attack by blocking incoming ICMP packets. This stopped the flood of traffic overwhelming the network. Shutting down non-critical services. This freed up resources to focus on critical operations. Security personnel will receive training on the new tools implemented, such as network monitoring software and source IP verification on the firewall. This ensures they can effectively utilize these resources. The incident response playbook will be updated to reflect the learnings from this event. Specifically, the "Detect" and "Protect" phases will be strengthened to address vulnerabilities related to ICMP traffic and firewall configuration.   |
| Recover | The DDoS attack resulted in a two-hour network outage, disrupting normal business operations. The IT and Security operations teams collaborated to restore network functionality and minimize downtime. The cybersecurity team shared information with staff and conducted a lessons learned session to: Analyze the root cause of the attack. Identify necessary safeguards to prevent future incidents. 
 |


# Notes <a name="notes"> 

This was a challenging exercise that I did really well. 

[The Understanding and Responding to Distributed Denial-of-Service Attacks whitepaper published by the CISA.](https://www.cisa.gov/sites/default/files/publications/understanding-and-responding-to-ddos-attacks_508c.pdf)


NIST article on suggestions for the properly recovering from a cyberattack
[How to Recover from a Cyber Attack | NIST](https://www.nist.gov/blogs/manufacturing-innovation-blog/how-recover-cyber-attack#:~:text=Consider%20Cyber%20Insurance%20for%20Increased%20Recovery%20Capability%20Like,assist%20in%20identifying%20the%20extent%20of%20damage%20caused)

# Reflections <a name="reflections"> 
This was a challenging exercise that I did really well . The part I struggled with was including too much and more detail 
