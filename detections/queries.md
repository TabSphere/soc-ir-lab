# 🔍 Detection Queries (Splunk SPL)

This file collects all Splunk SPL queries used in my SOC/IR Lab.  
Each query is documented with:  
- **Purpose** → Why this query matters in SOC operations.  
- **Alert Logic** → How it decides something is suspicious.  
- **MITRE ATT&CK Mapping** → Shows adversary technique coverage.  

---

## 🐝 Honeypot Detections

### 1. SSH Brute Force
```spl
index=syslog host=decoy-1 "SSH" 
| stats count by src_ip 
| where count > 10
