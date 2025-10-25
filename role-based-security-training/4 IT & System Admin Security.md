# 📘 Chapter 4 — IT & System Admin Security

*(Access Control | Patching | Privilege Misuse Prevention)*

---

## 🧠 Learning Objectives

By the end of this session, IT and support teams will be able to:
✅ Understand the critical role of IT admins in organizational security.
✅ Identify risks related to privileged accounts and access control failures.
✅ Implement a consistent patching and update policy.
✅ Prevent privilege escalation and insider misuse.
✅ Securely manage credentials, remote access, and system configurations.
✅ Build an auditable, least-privilege environment across users and systems.

---

## 📚 Slide / PDF Content — In Depth

---

### **Slide 1 — “Admins Hold the Keys to the Kingdom”**

> “With great power comes great responsibility — especially when your login can control every system.”

IT and System Admins have **super-user privileges** — making them **prime targets for attackers** and potential sources of internal mistakes.

💡 **Key Risks:**

* Privileged credential compromise
* Misconfigured systems (default passwords, open ports)
* Missed patches / unpatched software
* Insider misuse or accidental escalation
* Unsecured remote access (RDP, SSH)

🧩 **Case Example:**
A ransomware attack on a logistics company began when an IT admin reused a password across multiple servers — one credential leak led to complete domain compromise.

---

### **Slide 2 — Core Responsibilities of IT & SysAdmins**

| Area                  | Objective                       | Risk if Ignored                 |
| --------------------- | ------------------------------- | ------------------------------- |
| **Access Control**    | Limit rights to what users need | Privilege abuse, insider threat |
| **Patch Management**  | Keep OS, apps, firmware updated | Exploited vulnerabilities       |
| **System Hardening**  | Disable unnecessary services    | Backdoors & lateral movement    |
| **Monitoring & Logs** | Detect abnormal activities      | Missed breach indicators        |
| **Backup & Recovery** | Ensure data availability        | Ransomware loss                 |
| **Incident Response** | Quick containment of attacks    | Longer downtime                 |

🧩 **Trainer Demo:** Show an example of a misconfigured RDP port visible on Shodan → discuss impact.

---

### **Slide 3 — Access Control Best Practices (Zero Trust Model)**

| Practice                               | Description                                               |
| -------------------------------------- | --------------------------------------------------------- |
| **Least Privilege**                    | Give users the *minimum* rights they need.                |
| **Role-Based Access (RBAC)**           | Group permissions by job function (Admin, User, Auditor). |
| **Multi-Factor Authentication (MFA)**  | Required for all admin-level logins.                      |
| **Privileged Access Management (PAM)** | Use tools to control privileged credentials.              |
| **Account Review**                     | Disable unused or old admin accounts monthly.             |
| **Logging & Audit Trails**             | Track every admin action for accountability.              |

🧩 **Example:**

* Create separate accounts: `john_admin` for elevated tasks, `john_user` for normal work.
* Never use domain admin for daily tasks.

---

### **Slide 4 — Patching & Vulnerability Management**

> “Unpatched systems are open doors waiting to be used.”

| Step                       | Description                                            |
| -------------------------- | ------------------------------------------------------ |
| **1️⃣ Inventory Systems**  | Know every device, OS, app in your environment.        |
| **2️⃣ Monitor CVEs**       | Subscribe to NVD or vendor security bulletins.         |
| **3️⃣ Prioritize by Risk** | Critical vulnerabilities first (CVSS ≥ 8).             |
| **4️⃣ Automate Patching**  | Use WSUS, SCCM, or Ansible for updates.                |
| **5️⃣ Verify & Report**    | Log patch success, validate via vulnerability scanner. |

🧩 **Trainer Tip:** Show a live example of an outdated software → demonstrate patch application & CVE closure.

---

### **Slide 5 — Privilege Misuse & Insider Risk Prevention**

| Risk                        | Example                             | Defense                      |
| --------------------------- | ----------------------------------- | ---------------------------- |
| **Overprivileged Accounts** | Developers with domain admin rights | Role-based access control    |
| **Shared Admin Passwords**  | One password for all admins         | Use PAM or password vault    |
| **Command Abuse**           | Admin installs unauthorized tools   | Monitoring + approval policy |
| **Log Tampering**           | Admin clears logs after changes     | Centralized logging (SIEM)   |
| **Shadow IT**               | Use of unapproved SaaS tools        | Whitelisting policy          |

🧩 Real Case: Admin used PowerShell to extract HR data — unnoticed for 3 months due to missing audit logs.

---

### **Slide 6 — Remote Access & Endpoint Security**

| Area                     | Secure Practice                        |
| ------------------------ | -------------------------------------- |
| **RDP Access**           | Use VPN + MFA, disable if not required |
| **SSH / Telnet**         | Allow SSH only with key-based auth     |
| **Admin Workstations**   | Separate from regular desktops         |
| **Portable Devices**     | Encrypt drives with BitLocker / LUKS   |
| **USB Devices**          | Restrict or log all device connections |
| **Network Segmentation** | Isolate admin networks from users      |

🧩 Tip: Avoid using admin credentials on user systems — use temporary elevation tools instead.

---

### **Slide 7 — Patch Policy & Vulnerability Scanner Setup**

✔ Monthly patch window (e.g., second Saturday)
✔ Maintain patch log & report exceptions
✔ Use tools like:

* **Qualys / OpenVAS / Nessus** for vulnerability scans
* **WSUS / Ansible / Intune** for automated patch rollout
  ✔ Conduct quarterly system hardening audit

🧩 Activity: Scan a sample endpoint with OpenVAS and analyze vulnerabilities.

---

### **Slide 8 — Incident Response for Admins**

If you suspect compromise:

1️⃣ **Disconnect system** from network immediately.
2️⃣ **Inform Security / SOC team** — don’t fix silently.
3️⃣ **Preserve logs** for forensics.
4️⃣ **Change passwords** post-incident.
5️⃣ **Document everything** for audit and RCA.

🧩 Tip: Never hide admin errors — early reporting prevents escalation.

---

### **Slide 9 — Admin Security Checklist**

# | Task | Status

--|------|--------
1 | Maintain inventory of all admin accounts | ☐
2 | Enforce MFA for privileged access | ☐
3 | Patch OS and software monthly | ☐
4 | Disable unused services and ports | ☐
5 | Use PAM or vault for credentials | ☐
6 | Log and audit all admin actions | ☐
7 | Segregate admin network from user LAN | ☐
8 | Regular vulnerability scans | ☐
9 | Test backups quarterly | ☐
10 | Remove access of ex-employees | ☐

---

### **Slide 10 — Key Takeaways**

✅ Privileged accounts = biggest security risk if unmanaged.
✅ Follow *least privilege*, *MFA*, and *logging* as your golden trio.
✅ Patch consistently, automate when possible.
✅ Always separate duties: no single admin should have total control.
✅ Report issues early, document everything for audit readiness.

> “The best admins aren’t the ones who fix everything — they’re the ones who prevent the need to.” 🔐

---

## 🧩 Interactive Activities

| Activity                    | Description                                                  |
| --------------------------- | ------------------------------------------------------------ |
| **Privilege Audit Drill**   | List current admin accounts → identify overprivileged users. |
| **Patch Cycle Simulation**  | Demonstrate monthly patch deployment using test systems.     |
| **Access Review Challenge** | Review user permissions in AD and remove unnecessary roles.  |
| **Log Monitoring Workshop** | Analyze Windows Event Viewer or SIEM alerts.                 |

---

## 🧰 Recommended Tools for IT & Admin Security

| Tool                                         | Purpose                       | Platform       |
| -------------------------------------------- | ----------------------------- | -------------- |
| **OpenVAS / Qualys / Nessus**                | Vulnerability scanning        | Cross-platform |
| **CyberArk / BeyondTrust / Bitwarden Teams** | Privileged Access Management  | Enterprise     |
| **WSUS / Ansible / Intune**                  | Patch automation              | Windows/Linux  |
| **Graylog / Wazuh / ELK**                    | Centralized logging           | SIEM           |
| **BitLocker / LUKS**                         | Disk encryption               | Windows/Linux  |
| **CrowdStrike / Defender ATP**               | Endpoint detection & response | Enterprise     |

---

## 🧮 15 MCQs — IT & System Admin Security

**Q1.** Why are IT admins considered high-value targets?
A. They have limited data access
B. They control critical systems and data
C. They rarely use email
D. They work remotely
✅ **Answer: B**

**Q2.** What does “least privilege” mean?
A. Give everyone admin rights
B. Give minimum permissions needed to do the job
C. Disable all user accounts
D. Share one password for all
✅ **Answer: B**

**Q3.** Which tool is used for vulnerability scanning?
A. OpenVAS
B. MS Paint
C. Outlook
D. Zoom
✅ **Answer: A**

**Q4.** What is the purpose of PAM (Privileged Access Management)?
A. Backup data
B. Control and monitor admin credentials
C. Encrypt email
D. Clean temp files
✅ **Answer: B**

**Q5.** What should you do with inactive admin accounts?
A. Keep them for backup
B. Disable or delete them
C. Share with new employees
D. Ignore
✅ **Answer: B**

**Q6.** Why is patching important?
A. Improves aesthetics
B. Fixes vulnerabilities before exploitation
C. Speeds up the CPU
D. Reduces internet bills
✅ **Answer: B**

**Q7.** Which is a secure remote access practice?
A. Use VPN + MFA for RDP
B. Expose RDP to public IP
C. Share RDP password
D. Use Telnet without encryption
✅ **Answer: A**

**Q8.** What is a common privilege misuse example?
A. Installing unauthorized software
B. Checking email
C. Updating patches
D. Logging tickets
✅ **Answer: A**

**Q9.** What’s the best way to manage shared passwords?
A. Use a password vault or PAM
B. Store in Excel
C. Write on sticky note
D. Share via email
✅ **Answer: A**

**Q10.** Which security control ensures accountability?
A. Audit logging
B. File deletion
C. Anonymous access
D. Password sharing
✅ **Answer: A**

**Q11.** What’s the first step after detecting a system breach?
A. Report and isolate system
B. Reboot immediately
C. Delete logs
D. Ignore
✅ **Answer: A**

**Q12.** Why separate admin and user accounts?
A. Reduce attack surface
B. Easier to remember passwords
C. For decoration
D. To confuse attackers
✅ **Answer: A**

**Q13.** What does “patch cycle” refer to?
A. Periodic update and testing of systems
B. Installing antivirus
C. Powering on servers
D. Creating user accounts
✅ **Answer: A**

**Q14.** What is the goal of access control?
A. Restrict access to authorized users only
B. Allow everyone equal access
C. Store logs
D. Monitor bandwidth
✅ **Answer: A**

**Q15.** Which of these is part of incident response?
A. Documenting actions and evidence
B. Ignoring small alerts
C. Sharing logs publicly
D. Turning off all systems
✅ **Answer: A**

✅ **Answer Key:** 1B, 2B, 3A, 4B, 5B, 6B, 7A, 8A, 9A, 10A, 11A, 12A, 13A, 14A, 15A

---

## 🎯 Outcomes

✅ Admins understand and enforce least privilege and access control.
✅ Patching, monitoring, and incident response become consistent.
✅ Insider threats and misconfigurations are significantly reduced.
✅ Organization achieves audit-ready posture under ISO 27001 / SOC2.
✅ IT evolves from “support” to **secure infrastructure guardianship**.

> “Admins don’t just maintain systems — they maintain trust.” 🛡️

---

