# 📝 SOC/IR Lab Setup Log

This file documents each step I took while building my SOC & Incident Response lab.  
Keeping a log shows my troubleshooting process and progress.

---

## ✅ Environment
- Host: MacBook Pro (Bootcamp Windows 11)
- Virtualization: Oracle VirtualBox
- Network: Host-only Adapter

---

## 🖥️ Virtual Machines

### 1. Windows 11 (Endpoint)
- Source: Microsoft Eval ISO
- Status: Installed
- Next steps: Install Sysmon + Splunk Universal Forwarder

### 2. soc-splunk (Ubuntu Server)
- Source: Ubuntu Server 24.04 ISO
- Status: Pending
- Next steps: Install Splunk Enterprise

### 3. decoy-1 (Ubuntu Server Honeypot)
- Source: Ubuntu Server 24.04 ISO
- Status: Pending
- Next steps: Install OpenCanary

### 4. Kali Linux
- Source: Prebuilt VirtualBox OVA
- Status: Pending
- Next steps: Run test scans/attacks

---

## 🧩 To Do
- [ ] Configure Host-only networking across all VMs
- [ ] Confirm IP connectivity (ping test)
- [ ] Install Splunk Enterprise on soc-splunk
- [ ] Configure data forwarding from Windows + Honeypot
- [ ] Test detections with Kali attacks
