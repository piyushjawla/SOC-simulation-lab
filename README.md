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
