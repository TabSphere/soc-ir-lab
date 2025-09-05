# 🔍 Detection Queries (Splunk SPL)

This file collects all Splunk SPL queries used in my SOC/IR Lab.  
Each query is linked to the relevant detection use case and mapped to **MITRE ATT&CK** tactics & techniques.  

---

## 1. Honeypot SSH Brute Force
```spl
index=syslog host=decoy-1 "SSH" 
| stats count by src_ip 
| where count > 10
