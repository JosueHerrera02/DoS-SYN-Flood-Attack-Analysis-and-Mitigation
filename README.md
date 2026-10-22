# DoS-SYN-Flood-Attack-Analysis-and-Mitigation
Investigated a TCP SYN Flood attack through log analysis, identified indicators of compromise, and documented mitigation strategies.

## Objective
The objective of this project is to investigate and analyze a Denial of Service (DoS) SYN Flood attack by examining network logs, identifying indicators of malicious activity, and explaining how the attack disrupted normal website operations. Through the analysis of repeated TCP SYN requests originating from a single source IP address, this project demonstrates the impact of a SYN Flood attack on server availability and highlights mitigation strategies to reduce the risk of similar incidents in the future.

### Skills Learned
- Network Traffic Analysis
- TCP/IP Fundamentals and Three-Way Handshake Analysis
- Detection of Denial of Service (DoS) Attacks
- SYN Flood Attack Identification
- Log Analysis and Interpretation
- Incident Investigation and Documentation
- Identification of Indicators of Compromise (IoCs)
- Security Monitoring and Threat Detection
- Root Cause Analysis
- Cybersecurity Incident Response
- Network Security Concepts
- Mitigation and Remediation Planning
- Technical Report Writing
- Critical Thinking and Problem Solving


### Tools Used
- tcpdump – Network packet capture and traffic analysis
- TCP Protocol Analysis – Investigation of SYN packet behavior
- Network Logs – Review and analysis of connection attempts
- Firewall Rules (research/mitigation) – IP blocking and traffic filtering strategies

## Steps
- 1. Reviewed the incident report and identified the service disruption affecting the web server.
- 2. Analyzed network log data to identify suspicious traffic patterns.
- 3. Examined TCP traffic and observed a high volume of SYN packets from a single source IP address (203.0.113.0).
- 4. Verified that the traffic targeted a single destination server (192.0.2.1) within a very short time frame.
- 5. Determined that the activity matched the characteristics of a DoS SYN Flood attack.
- 6. Investigated how the attack exploited the TCP three-way handshake process to overwhelm server resources.
- 7. Assessed the impact on website availability and user connectivity.
- 8. Documented findings, indicators of compromise (IoCs), and attack behavior.
- 9. Researched mitigation strategies, including firewall rules to block malicious IP addresses and reduce the risk of similar attacks.
- 10. Produced an incident report summarizing the analysis, findings, and recommended remediation measures
