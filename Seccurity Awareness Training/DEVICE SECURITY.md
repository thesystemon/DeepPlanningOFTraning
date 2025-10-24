# 📘 **Chapter 5 — DEVICE SECURITY (Laptops, Mobiles, USBs)**

---

## 🧠 **Learning Objectives**

By the end of this module, employees will be able to:

* Protect company and personal devices from theft, misuse, or malware infection.
* Understand the risks of unprotected laptops, mobiles, and removable media.
* Apply encryption, auto-lock, and secure connection practices.
* Recognize unsafe device behaviors (plugging unknown USBs, using public Wi-Fi, etc.).
* Respond correctly when a device is lost, stolen, or compromised.

---

## 📚 **Slide / PDF Content — In Depth**

---

### **Slide 1 — “Your Device = Your Gateway to the Company”**

> “If your device is compromised, your company is compromised.”

Every laptop, phone, or tablet is a **doorway to company data** — even if you’re just checking email or Slack.
Hackers don’t need to hack the server if they can infect your device first.

---

### **Slide 2 — Common Device Security Risks**

| Threat                    | Description                      | Example                                    |
| ------------------------- | -------------------------------- | ------------------------------------------ |
| **Theft / Loss**          | Unattended devices can be stolen | Laptop left in taxi or café                |
| **Malware / Keyloggers**  | From untrusted downloads or USBs | Free “video converter” tool infects device |
| **Unpatched Systems**     | Old software vulnerabilities     | Windows not updated → ransomware entry     |
| **Unsafe Wi-Fi**          | Public Wi-Fi interception        | Attacker sniffs traffic at coffee shop     |
| **Removable Media Risks** | Infected USB drives              | “Free USB” found → contains malware        |

🧩 *Trainer Demo:*
Show a short video or simulation — infected USB auto-executes malware (safe demo using dummy file).

---

### **Slide 3 — Laptop Security Best Practices**

✅ **Lock Your Screen:**
Always lock before leaving your desk — shortcut keys:

* Windows → `Win + L`
* macOS → `Ctrl + Cmd + Q`

✅ **Encrypt Your Hard Drive:**

* Windows: *BitLocker*
* macOS: *FileVault*
  Encryption ensures data can’t be accessed even if device is stolen.

✅ **Keep Software Updated:**

* Enable automatic OS and antivirus updates.
* Outdated software = open door for attackers.

✅ **Avoid Using Local Admin Rights:**
Use standard user account to reduce malware damage.

✅ **Back Up Regularly:**
Use cloud backups (OneDrive, Google Drive, or company server).

---

### **Slide 4 — Mobile Device Security**

Your phone holds sensitive data — emails, chats, files, MFA apps.
It needs the same level of protection as your laptop.

**Best Practices:**
📱 Enable **strong PIN, fingerprint, or face unlock**
📱 **Install apps only from official stores** (Google Play / App Store)
📱 **Disable Bluetooth & Wi-Fi** when not in use
📱 **Turn off auto-connect** to public Wi-Fi networks
📱 **Avoid jailbreaking / rooting** devices
📱 **Use MDM (Mobile Device Management)** if provided by company
📱 **Enable remote wipe** (Find My Device / Find My iPhone)

🧩 *Case Study:*
Employee lost phone with business WhatsApp — attacker accessed client data.
After training, company enforced MDM + auto remote wipe → prevented future breach.

---

### **Slide 5 — USB & Removable Media Security**

USB drives = one of the oldest, simplest infection methods.

⚠️ **Risks:**

* Malware autorun on insertion
* Data leakage via copying sensitive files
* Physically lost USBs exposing confidential info

**Safety Rules:**
✅ Only use **company-approved USB drives**
✅ **Scan USBs** with antivirus before opening
✅ **Disable autorun** feature in OS
✅ **Encrypt sensitive data** on USBs (use VeraCrypt / BitLocker To Go)
✅ **Never use found or gifted USB drives**

🧩 *Trainer Demo:*
Show example: “Free USB dropped in office parking lot” → 80% of people plug it in (real stat!).

---

### **Slide 6 — Public Wi-Fi & Remote Work Risks**

**Why Public Wi-Fi is Dangerous:**

* Traffic can be intercepted using simple sniffing tools (like Wireshark).
* Fake “Free Wi-Fi” hotspots can capture logins.

**Protection Tips:**
✅ Use **VPN (ProtonVPN, Windscribe – free versions available)**
✅ Never log in to work email or banking on open networks
✅ Use **mobile hotspot** if possible
✅ Turn off **file sharing** when traveling

🧩 *Trainer Demo:*
Show “Man-in-the-Middle” diagram to explain Wi-Fi data interception visually.

---

### **Slide 7 — Physical Security at Workplace**

🔒 Don’t leave laptops unlocked on desks.
🪑 Use **security cable locks** when traveling.
🧍‍♂️ Don’t allow “tailgating” (someone entering with you).
💼 Store USBs and drives in locked drawers.
📸 Don’t click or record company screens with personal phones.

🧩 *Visual Activity:*
Show 5 pictures — identify poor device security habits (e.g., unlocked PC, USB left in port).

---

### **Slide 8 — What To Do If Device is Lost / Stolen**

**Immediate Steps:**

1. Report to IT/Security team (email, call hotline).
2. If possible, trigger **remote wipe** or **lock**.
3. Change passwords linked to that device (email, VPN, apps).
4. File police report (for audit and legal proof).

**Don’t try to recover it alone.**
**Never delay reporting** — time matters.

---

### **Slide 9 — Organizational Security Controls**

* Enforced BitLocker/FileVault encryption
* Automatic screen lock after 5 minutes idle
* USB port control policies
* Mobile Device Management (MDM) for smartphones
* Endpoint Detection & Response (EDR)
* Zero Trust access control for remote workers

---

### **Slide 10 — Key Takeaways**

✅ Treat every device as a **company asset**.
✅ Lock, encrypt, and back up.
✅ Avoid plugging unknown devices.
✅ Always report lost or suspicious behavior immediately.

> “Device security = personal responsibility + company policy.”

---

## 🧩 **Interactive Activities**

| Activity              | Description                                                          |
| --------------------- | -------------------------------------------------------------------- |
| **Spot the Risk**     | Trainer shows images of insecure setups — employees identify issues. |
| **USB Simulation**    | Demonstrate how autorun malware spreads using a dummy USB.           |
| **Encryption Demo**   | Show how to enable BitLocker/FileVault.                              |
| **Lost Device Drill** | Simulate a “lost laptop” scenario — test response speed.             |

---

## 🧰 **Free & Open-Source Tools You Can Use**

| Tool                                       | Purpose                | Type                 |
| ------------------------------------------ | ---------------------- | -------------------- |
| **VeraCrypt**                              | USB & drive encryption | Free / Open Source   |
| **ProtonVPN / Windscribe**                 | Secure Wi-Fi browsing  | Free                 |
| **BitLocker / FileVault**                  | Full-disk encryption   | Built-in             |
| **Windows Defender / ClamAV**              | Malware protection     | Free                 |
| **MDM (Intune for Education / Flyve MDM)** | Mobile management      | Freemium/Open Source |
| **USBDeview**                              | Track USB device usage | Free                 |
| **Google Find My Device / Apple iCloud**   | Remote lock/wipe       | Free                 |

---

## 🧮 **15 MCQs — Device Security Awareness**

---

**Q1.** What should you do before leaving your desk?
A. Lock your screen
B. Keep it open for convenience
C. Let a friend use your PC
D. Turn off monitor only
✅ **Answer:** A — Always lock screen using `Win+L` or `Ctrl+Cmd+Q`.

---

**Q2.** What is BitLocker used for?
A. Browsing securely
B. Encrypting hard drives
C. Cleaning malware
D. Blocking ads
✅ **Answer:** B — BitLocker encrypts data to prevent unauthorized access.

---

**Q3.** Which of the following is unsafe behavior?
A. Using approved USBs
B. Using found USB drives
C. Scanning drives with antivirus
D. Encrypting sensitive data
✅ **Answer:** B — Never use unknown or found USBs.

---

**Q4.** How often should you update your software?
A. When system asks or automatically
B. Once a year
C. Never, to save time
D. Only if infected
✅ **Answer:** A — Always keep updates on auto mode.

---

**Q5.** Public Wi-Fi should be used only when:
A. You use a secure VPN
B. You share files
C. You check banking
D. You log into work account
✅ **Answer:** A — VPN encrypts your data over unsafe Wi-Fi.

---

**Q6.** What is MDM?
A. Mobile Device Management
B. Malware Detection Mechanism
C. Multi Data Monitoring
D. Master Device Module
✅ **Answer:** A — It secures and monitors mobile devices in organizations.

---

**Q7.** Why should autorun be disabled?
A. Prevent USB drives from executing malware automatically
B. Save power
C. Faster boot
D. Cleaner desktop
✅ **Answer:** A — Autorun can execute malicious files automatically.

---

**Q8.** Which shortcut locks your screen instantly?
A. Ctrl + Alt + Del
B. Win + L (Windows) / Ctrl + Cmd + Q (Mac)
C. Ctrl + Shift + X
D. F5
✅ **Answer:** B — These shortcuts lock the screen quickly.

---

**Q9.** What is the safest way to back up data?
A. Store on personal USB
B. Use approved cloud or company backup drive
C. Email to yourself
D. None
✅ **Answer:** B — Use official backup systems.

---

**Q10.** When should you report a lost device?
A. Immediately
B. After 2 days
C. Only if it’s expensive
D. When asked
✅ **Answer:** A — Early reporting reduces damage.

---

**Q11.** Which practice protects mobile data best?
A. Strong PIN / biometric unlock
B. Auto-connect to Wi-Fi
C. Install random apps
D. Disable screen lock
✅ **Answer:** A — Always use strong authentication.

---

**Q12.** What’s the main risk with removable media?
A. Inconvenience
B. Malware & data theft
C. Battery drain
D. Slower PC
✅ **Answer:** B — USBs can spread malware and leak data.

---

**Q13.** Which security layer protects device even after theft?
A. Encryption
B. Wallpaper password
C. Screen brightness
D. None
✅ **Answer:** A — Encryption keeps data unreadable.

---

**Q14.** What should you avoid in public Wi-Fi?
A. Checking email
B. File sharing
C. Logging into sensitive accounts without VPN
D. All of the above
✅ **Answer:** D — All unsafe activities without VPN.

---

**Q15.** What to do if a coworker plugs unknown USB in office PC?
A. Ignore
B. Warn and report to IT immediately
C. Check it yourself
D. Format PC
✅ **Answer:** B — Report to IT/SOC right away.

---

✅ **Answer Key:** 1A, 2B, 3B, 4A, 5A, 6A, 7A, 8B, 9B, 10A, 11A, 12B, 13A, 14D, 15B

---

## 📊 **Measurement & Client Reporting**

| Metric                      | Description               |
| --------------------------- | ------------------------- |
| % of encrypted devices      | Should reach ≥90%         |
| Lost device reports         | Should decrease quarterly |
| Quiz performance            | ≥80% average score        |
| Public Wi-Fi/VPN compliance | ≥70% usage in audits      |

---

## 🎯 **Final Outcomes**

✅ Employees secure all endpoints (laptops, phones, USBs).
✅ Fewer malware infections and data leaks.
✅ Higher compliance with company device policy.
✅ Enhanced security posture for hybrid & remote work culture.

---
