# SOC-simulation-lab
Simulating a Security Operations Center (SOC) using log analysis and attack detection.

## Objective
To simulate a Security Operations Center (SOC) by generating, collecting and analyzing logs to detect suspicious activities.

## Architecture
- Windows Server (Domain Controller)
- Windows Client machine
- Kali Linux (Attacker)
- Splunk (Log Monitoring)

## Learning Goals
- Understand how logs are generated
- Learn how attacks appear in logs
- Detect suspicious behaviour using SIEM tools

## Progress Log
### Day 1: Project initialized, planning architecture.

### Day 2: Network architecture enhancement
- Configured dual network adapters on domain controller
- Maintained internal network for domain communication
- Added NAT adapter for internet access
- Ensured network isolation between lab environment and external internet

### Switched SIEM Approach
- Identified limitations with Splunk licensing for homelab
- Researched alternatives
- Selected Wazuh as the open-source SIEM solution

### Handling OS compatibility issue
- Encountered OS compatibility restrictions during Wazuh installation
- Verified Ubuntu version
- Used `--ignore-check` flag to bypass installer restriction (safe for homelab)

### Wazuh deployment progress
- Successfully initiated Wazuh installation
- Verified dashboard service startup

### Network configuration for Wazuh server
- Identified missing IP on internet network interface
- Manually configured static IP for LabNet adapter
- Ensured connectivity between domain controller, client, and SIEM server
- Identified that internal network is isolated from host machine
- Implemented NAT port forwarding to expose Wazuh dashboard
- Enabled secure access to SIEM interface via localhost
