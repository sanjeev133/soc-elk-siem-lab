# soc-elk-siem-lab

In this project, I built and configured a SIEM solution using the ELK Stack (Elasticsearch, Logstash, Kibana) to simulate a real-world Security Operations Center (SOC) environment.
The goal was to understand how security teams collect logs, detect threats, investigate incidents, and monitor infrastructure health in a centralized system.
Through this hands-on setup, I gained practical experience in log management, detection engineering, troubleshooting, and security monitoring.
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
# Tools & Technologies Used

    - Elasticsearch
    - Logstash
    - Kibana
    - Filebeat / Elastic Agent
    - Ubuntu Server 24.0 (Linux)
    - Windows Event Logs
    - VirtualBox (Lab Environment)
    - SSL/TLS Certificate Configuration (.PEM)
    - Kibana Query Language (KQL)
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 # Architecture

The environment was built using the following flow:
Log Sources (Windows/Linux machines)
→ Filebeat / Elastic Agent
→ Logstash (log parsing & filtering)
→ Elasticsearch (indexing & storage)
→ Kibana (visualization & investigation)

# This setup allowed centralized monitoring and efficient threat analysis.

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
# Key Features Implemented

-> Centralized log collection from Windows and Linux systems
-> Log parsing and normalization using Logstash filters
-> Secure communication using SSL certificates
-> User authentication and access control using X-Pack security
-> Custom dashboards in Kibana for monitoring security events
-> Detection queries using KQL
-> Cluster health monitoring and troubleshooting

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
# Security Use Cases Implemented

# Failed Login Detection
  Monitored Windows Event ID 4625 to detect repeated failed login attempts and possible brute-force activity.
  
# Port Scanning Detection
  Analyzed unusual connection patterns indicating scanning activity.

# Cluster Health Monitoring
  Monitored Elasticsearch cluster states (green, yellow, red) and resolved issues when necessary.

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# Lab Environment Details

Single-node deployment.
Bridge networking .
Elasticsearch running on port 9200.
Kibana running on port 5601.
Security enabled with X-Pack.
Self-signed certificates for secure communication.

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# Challenges & Troubleshooting

During implementation, I encountered and resolved:

Red cluster state issues.
SSL certificate configuration errors.
Authentication and credential recovery problems
Logstash pipeline parsing errors
Service failures analyzed using journalctl -xeu and reading logs.

# These challenges helped strengthen my debugging and problem-solving skills.

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# Skills Demonstrated

SIEM deployment and configuration.
Log analysis and threat detection.
SOC monitoring workflow.
Incident investigation.
Elasticsearch troubleshooting.
Linux system administration.
Network traffic analysis.
Security dashboard development.

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

** Key Learnings
This project gave me practical exposure to how a SOC operates in real-world environments. I learned how logs are ingested, parsed, analyzed, and used to detect malicious     activity. I also gained confidence in configuring secure environments and resolving infrastructure issues.**
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
# Future Improvements

  - Integration with Suricata IDS
  - Adding threat intelligence feeds
  - Implementing automated alert notifications
  - Deploying a multi-node cluster
  - Containerizing the ELK stack using Docker
  
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------
**Author
**Sanjeev Choudhary
Aspiring SOC Analyst | Cybersecurity Enthusiast****
