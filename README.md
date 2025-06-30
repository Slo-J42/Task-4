
 🔥 Firewall Configuration and Testing (Linux/Windows)

 🎯 Objective
To configure and test basic firewall rules using built-in tools on both Linux and Windows systems. The goal is to understand how to allow and block network traffic effectively to enhance system security.

---

## 🛠️ Tools Used

 Platform - Tool 

 Linux - UFW (Uncomplicated Firewall) 


---

 📋 Task Steps (UFW – Kali Linux)

1. **Check Firewall Status**
   ```bash
   sudo ufw status verbose
   ```

2. **List Current Rules**
   ```bash
   sudo ufw status numbered
   ```

3. **Block Telnet Port (23)**
   ```bash
   sudo ufw deny 23
   ```

4. **Test Port Block**
   ```bash
   telnet localhost 23
   ```

5. **Allow SSH (Port 22)**
   ```bash
   sudo ufw allow ssh
   ```

6. **Remove Telnet Block Rule**
   ```bash
   sudo ufw delete deny 23
   ```

7. **Export Rule Set**
   ```bash
   sudo ufw status verbose > ufw_rules.txt
   ```

---

📸 Deliverables

- `Firewall_Configuration_Report.pdf`: Detailed step-by-step guide.
- Screenshots : Visual evidence of rule application and testing.

---

 🧠 Summary

This task demonstrates basic firewall management skills:
- Blocking insecure protocols (e.g., Telnet).
- Allowing secure traffic (e.g., SSH).
- Verifying firewall behavior.
