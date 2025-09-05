# 🛡️ SOC / Incident Response Lab

This is my hands-on **SOC & Incident Response home lab project**.  
It simulates a real SOC environment using:

- **Splunk SIEM** (log collection & detection)
- **Windows 11 Endpoint** (Sysmon + Splunk Forwarder)
- **OpenCanary Honeypot** (deception logging)
- **Kali Linux** (attacker machine)

---

## 📖 Goals
- Practice SOC analyst workflows (detection, triage, escalation).
- Build detections using real attack telemetry.
- Write professional Incident Response reports.
- Showcase blue team skills for security job interviews.

---

## 🏗️ Architecture

[ Kali Attacker ] ───▶ [ OpenCanary Honeypot ]
│ │
└──────▶ [ Windows Endpoint ]
│
▼
[ Splunk SIEM ]

![SOC IR Lab Architecture](screenshots/architecture.png)


## 📂 Repo Contents
- `configs/` → Lab configs (Splunk, Sysmon, OpenCanary).
- `detections/` → Splunk SPL queries, dashboards.
- `reports/` → Incident Reports with MITRE ATT&CK mapping.
- `screenshots/` → Evidence from the lab.
- `notes/` → Setup notes, troubleshooting.

---

## 🚀 Next Steps
- [ ] Install Splunk server (soc-splunk VM).
- [ ] Configure Windows endpoint logging (Sysmon + Splunk Forwarder).
- [ ] Deploy honeypot with OpenCanary.
- [ ] Simulate attacks from Kali.
- [ ] Detect and document incidents.

---

## 🧠 Skills Demonstrated
- SIEM deployment and log collection
- Endpoint telemetry enrichment with Sysmon
- Honeypot deception for early detection
- Writing SPL queries and building dashboards
- End-to-end Incident Response workflow
- Documentation and reporting mapped to MITRE ATT&CK

---

## 📌 Notes
This repo will grow as I build out the lab.  
Stay tuned for configs, detections, screenshots, and professional IR reports.
