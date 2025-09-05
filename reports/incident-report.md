# 🚨 Incident Report

## 📌 Summary
- **Date of Incident:** YYYY-MM-DD
- **Reported By:** (Your SOC Analyst name)
- **Affected Systems:** Windows Endpoint, Honeypot
- **Severity:** High / Medium / Low

---

## 🕒 Timeline
| Time (UTC) | Event |
|------------|-------|
| 10:05 | Suspicious scan detected from attacker IP |
| 10:10 | SSH brute force attempt on honeypot |
| 10:15 | Failed logon attempts on Windows endpoint |
| 10:20 | Suspicious PowerShell execution detected |

---

## 🔎 Detection
- **Splunk Queries Used:**  
  - Honeypot SSH brute force detection  
  - Windows failed logons (EventCode 4625)  
  - Suspicious PowerShell (encoded commands)

- **Screenshots:**  
  - Attach screenshots from Splunk searches or dashboards

---

## 🚨 Analysis
- **Attacker IP:** 192.168.56.xxx  
- **TTPs Observed:**  
  - Brute Force (MITRE ATT&CK T1110)  
  - PowerShell Execution (T1059.001)  
  - Reconnaissance (T1046)  

---

## 🛡️ Response
- Containment: Isolated affected endpoint  
- Eradication: Blocked attacker IP in firewall  
- Recovery: Reset affected credentials, restored VM snapshot  

---

## 📚 Lessons Learned
- Detection gaps found: (e.g. no alert for SMB enumeration)  
- Improvements: Add correlation rules, tighten alert thresholds  
