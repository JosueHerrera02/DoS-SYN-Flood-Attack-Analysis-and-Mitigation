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
You can have access to the tcpdump log <a href="https://www.dropbox.com/scl/fi/8zzljfyzlbp4uu07nd3pk/tcpdump_log.xlsx?rlkey=3k22nosqhxf3u7z95wpohu96u&st=6xqi6lfj&dl=0">here</a>
- 2. Analyzed network log data to identify suspicious traffic patterns.
- 3. Examined TCP traffic and observed a high volume of SYN packets from a single source IP address (203.0.113.0).
Note: if you have not downloaded the tcpdump file, here is a <a href="//imgur.com/a/Dx7UQcU">screenshot</a>
- 4. Verified that the traffic targeted a single destination server (192.0.2.1) within a very short time frame.
- 5. Determined that the activity matched the characteristics of a DoS SYN Flood attack. The Source IP address (203.0.113.0) was sending thousands of SYN requests to the Destination IP address (192.0.2.1) which in this case is the server.
- 6. Investigated how the attack exploited the TCP three-way handshake process to overwhelm server resources. 1. SYN — Client → Server (The client sends a SYN (synchronize) packet to the server to request a connection and propose an initial sequence number). 2. SYN‑ACK — Server → Client (The server responds with SYN‑ACK, acknowledging the client’s SYN and sending its
own SYN back to establish its sequence number). 3.ACK — Client → Server (The client sends a final ACK (acknowledgment) to confirm the server’s SYN‑ACK. At this point, the connection is fully established and data transfer can begin).
- 7. Assessed the impact on website availability and user connectivity. The users had no access to the website
- 8. Documented findings, indicators of compromise (IoCs), and attack behavior. You can have access to such incident report <a href="//imgur.com/a/yVkr3u1">here</a>
- 9. Researched mitigation strategies, including firewall rules to block malicious IP addresses and reduce the risk of similar attacks.
- 10. Produced an incident report summarizing the analysis, findings, and recommended remediation measures
