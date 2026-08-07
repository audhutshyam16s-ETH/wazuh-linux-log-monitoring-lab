Project Title
SOC Home Lab – Linux Log Monitoring using Wazuh
Overview

Example:

Built a SOC Home Lab using Wazuh to monitor Ubuntu Linux endpoints. Configured centralized log collection, File Integrity Monitoring (FIM), Security Configuration Assessment (SCA), and analyzed security events using the MITRE ATT&CK framework.

Architecture
               Kali Linux
            (Attack Machine)
                    │
        SSH / Nmap / Hydra
                    │
                    ▼
      Ubuntu Agent (192.168.0.105)
                    │
         Wazuh Agent collects logs
                    │
                    ▼
     Ubuntu Manager (192.168.0.102)
                    │
                    ▼
          Wazuh Dashboard
Technologies Used
Ubuntu Server 24.04 LTS
Wazuh 4.13.1
VirtualBox
Kali Linux
Linux
SSH
File Integrity Monitoring
Security Configuration Assessment
MITRE ATT&CK
Features
Linux authentication monitoring
SSH failed login detection
File Integrity Monitoring
Security Configuration Assessment
User creation monitoring
Package installation monitoring
Sudo monitoring
MITRE ATT&CK mapping
Skills Demonstrated
Linux Administration
SIEM
Log Analysis
Threat Hunting
Incident Investigation
Endpoint Monitoring
MITRE ATT&CK
SOC Operations
Screenshots to Include

Take screenshots of:

Wazuh Dashboard
Active Ubuntu Agent
Threat Hunting
SSH Failed Login Alert
MITRE ATT&CK Mapping
FIM Alert
User Creation Alert
SCA Dashboard
Architecture Diagram

You can create a simple diagram like:

             Kali Linux
                 │
                 ▼
          Ubuntu Agent
                 │
          Wazuh Agent
                 │
                 ▼
         Wazuh Manager
                 │
                 ▼
         Wazuh Dashboard
