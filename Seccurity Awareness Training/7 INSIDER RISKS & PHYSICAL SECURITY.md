# 📘 **Chapter 7 — INSIDER RISKS & PHYSICAL SECURITY**

---

## 🧠 **Learning Objectives**

By the end of this module, employees will:

* Understand what **insider risk** means and how it differs from external threats.
* Recognize that not all insider threats are intentional — some happen by mistake.
* Learn safe **physical security practices** to protect assets, devices, and data.
* Know how to **detect and report suspicious internal behavior** early.
* Apply the **"Zero Trust Mindset"** — trust, but always verify.

---

## 📚 **Slide / PDF Content (Trainer Material in Depth)**

---

### **Slide 1 — What Are Insider Risks?**

> “Not every attack comes from outside. Sometimes, danger is sitting right next to us.”

🔹 **Definition:**
An insider risk occurs when an employee, contractor, or trusted partner misuses access — intentionally or accidentally — leading to data loss, theft, or system damage.

🔹 **Types of Insiders:**

* **Malicious Insider** → Acts deliberately (revenge, money, ideology).
* **Negligent Insider** → Careless mistakes (sharing credentials, misconfiguring systems).
* **Compromised Insider** → Account hacked by an attacker using phishing or malware.

🧩 *Example Story:*
A finance staff member clicked a phishing link → their email was compromised → attacker sent fake payment instructions to vendors.
→ *Result:* ₹40 lakhs loss before IT detected it.

---

### **Slide 2 — Common Insider Risk Scenarios**

| Scenario                               | Risk Type   | Example                                |
| -------------------------------------- | ----------- | -------------------------------------- |
| Sharing credentials                    | Negligent   | “Hey, use my login just for a minute.” |
| Downloading client data to USB         | Negligent   | Data leakage via personal device       |
| Disgruntled ex-employee deleting files | Malicious   | Revenge attack                         |
| Developer uploading code to GitHub     | Negligent   | Source code exposure                   |
| Phished employee credentials used      | Compromised | Attacker gains internal access         |

---

### **Slide 3 — Why Do Insider Incidents Happen?**

💡 **Top Reasons:**

* Weak access control (no MFA)
* Poor offboarding (ex-employee access not revoked)
* Lack of awareness
* Unsecured physical environment
* Personal devices (BYOD) not managed

---

### **Slide 4 — Physical Security Basics**

> “Cybersecurity starts at the door.”

Physical access to your office, data center, or even a laptop = direct path to compromise.

**Golden Rules:**

* Always wear your company ID card.
* Never let unknown visitors tailgate (follow you into secure areas).
* Lock your computer screen when stepping away (Win+L).
* Keep laptops & USBs secured — don’t leave them unattended.
* Protect access cards — don’t lend or share them.
* Secure meeting rooms, server racks, and network equipment.

🧩 *Trainer Demo:*
Show short video: a person tailgating behind someone through an access door.
Ask: “Would you stop this person?”

---

### **Slide 5 — Clean Desk & Clear Screen Policy**

> “What’s left on your desk can be stolen faster than what’s on your desktop.”

✅ Always:

* Store confidential papers in locked drawers.
* Shred documents when not needed.
* Don’t stick passwords on monitors or under keyboards.
* Log off or lock screen before leaving desk.
* Remove USBs or drives when not in use.

🧩 *Practical Demo:*
Trainer hides a fake “password note” under a keyboard during session → see who spots it first.

---

### **Slide 6 — Data & Device Protection**

* Use company-approved devices only.
* Don’t connect unknown USB drives.
* Keep device OS and antivirus updated.
* Encrypt laptops (BitLocker, FileVault).
* Disable Bluetooth when not needed.
* Report lost/stolen devices immediately.

🧩 *Example Incident:*
Employee left laptop in a café → stolen → contained client PII without encryption.
Result: Breach notification + ₹10 lakh compliance penalty.

---

### **Slide 7 — Visitors & Contractors Policy**

🚫 Don’t let unknown people enter restricted zones.
🪪 Escort all visitors — they must sign in/out.
📸 Do not allow photography in secure areas.
🔒 Lock meeting rooms and storage after use.
🧾 Verify identity of service vendors and delivery personnel.

---

### **Slide 8 — Recognizing Suspicious Behavior**

Watch for:

* Unusual data downloads (large file transfers).
* Unauthorized USB use.
* Accessing systems outside work hours.
* Complaints about management and threats of revenge.
* Attempts to disable security controls.

⚠️ **Report quietly** to IT or HR — don’t confront the person directly.

---

### **Slide 9 — Response to Insider Incidents**

If you suspect insider misuse:
1️⃣ Report immediately to Security/IT/HR.
2️⃣ Do not delete or alter evidence.
3️⃣ Log time, actions, and any messages related to incident.
4️⃣ Cooperate during investigation — confidentiality is key.

---

### **Slide 10 — Key Takeaways**

✅ Insider threats are real — intentional or accidental.
✅ Lock screens, drawers, and doors.
✅ Verify identity before sharing or granting access.
✅ Follow “Clean Desk, Clear Screen.”
✅ Report suspicious activities early — prevention is cheaper than cure.

> “Security culture = when every employee acts like a security guard.”

---

## 🧩 **Interactive Activities**

| Activity                     | Description                                                            |
| ---------------------------- | ---------------------------------------------------------------------- |
| **Tailgating Drill**         | Trainer walks behind employees through the office — who challenges it? |
| **Clean Desk Challenge**     | Teams inspect each other’s desks for visible data or devices.          |
| **Suspicious Behavior Game** | Show short case videos → employees identify risk signs.                |
| **Device Lock Speed Test**   | Employees lock screens as fast as possible; leaderboard created.       |

---

## 🧰 **Free / Low-Cost Tools for Physical & Insider Risk Awareness**

| Tool                        | Purpose                                  | Platform      |
| --------------------------- | ---------------------------------------- | ------------- |
| **Canva / Google Slides**   | Create posters: “Lock It, Don’t Lose It” | Web           |
| **BitLocker / VeraCrypt**   | Device encryption                        | Windows/macOS |
| **USBDeview (NirSoft)**     | Check unauthorized USB connections       | Windows       |
| **AuditPol / Event Viewer** | Log insider activities                   | Windows       |
| **Security Onion / Wazuh**  | Detect unusual internal access           | Open-source   |
| **ZoneMinder**              | Free CCTV management                     | Linux         |
| **Google Forms**            | Anonymous insider report form            | Web           |

---

## 🧮 **15 MCQs — Insider Risk & Physical Security Awareness**

---

**Q1.** What is an insider threat?
A. Only hackers outside the organization
B. Anyone within the company who misuses access
C. Physical theft by strangers
D. Malware infection
✅ **Answer:** B

---

**Q2.** Which is an example of a negligent insider?
A. Employee leaks data intentionally
B. Employee clicks phishing link accidentally
C. Hacker compromises network
D. Vendor bypasses firewall
✅ **Answer:** B

---

**Q3.** What is tailgating?
A. Following someone through a secure door without authorization
B. Sending phishing emails
C. Copying data to USB
D. Talking on phone in secure areas
✅ **Answer:** A

---

**Q4.** What’s the first step when you suspect insider misuse?
A. Ignore it
B. Confront the person
C. Report quietly to IT/Security/HR
D. Announce publicly
✅ **Answer:** C

---

**Q5.** Which of these should never be done with visitor badges?
A. Collected at exit
B. Shared among employees
C. Issued by security
D. Worn visibly
✅ **Answer:** B

---

**Q6.** What’s the purpose of “Clean Desk Policy”?
A. Make office tidy
B. Prevent confidential data exposure
C. Save paper
D. Encourage minimalism
✅ **Answer:** B

---

**Q7.** Which physical security practice is correct?
A. Leave door open for delivery guy
B. Lock workstation when away
C. Keep passwords on sticky notes
D. Share access card
✅ **Answer:** B

---

**Q8.** What type of insider intentionally steals or damages data?
A. Negligent
B. Malicious
C. Compromised
D. Temporary
✅ **Answer:** B

---

**Q9.** What’s the risk of using unknown USBs?
A. Device may overheat
B. Malware or data theft
C. Slower system
D. Nothing serious
✅ **Answer:** B

---

**Q10.** Who is responsible for reporting suspicious activity?
A. Only IT staff
B. Security guards
C. Every employee
D. CEO only
✅ **Answer:** C

---

**Q11.** What should you do if your ID badge is lost?
A. Ignore it
B. Report immediately and get it blocked
C. Borrow someone else’s
D. Continue entering normally
✅ **Answer:** B

---

**Q12.** What’s the best action after noticing an unauthorized person in the office?
A. Ask for ID or inform security
B. Take photo and post online
C. Ignore it
D. Help them enter
✅ **Answer:** A

---

**Q13.** What’s one example of malicious insider behavior?
A. Clicking link by mistake
B. Deleting company files out of anger
C. Forgetting to log out
D. Losing access card
✅ **Answer:** B

---

**Q14.** What’s the function of BitLocker?
A. Encrypt data on laptops
B. Detect malware
C. Delete temporary files
D. Manage passwords
✅ **Answer:** A

---

**Q15.** Why should devices be locked when unattended?
A. To save battery
B. To prevent unauthorized access
C. To make desk look clean
D. No reason
✅ **Answer:** B

✅ **Answer Key:** 1B, 2B, 3A, 4C, 5B, 6B, 7B, 8B, 9B, 10C, 11B, 12A, 13B, 14A, 15B

---

## ✅ **Insider Risk & Physical Security Checklist (Employee Self-Assessment)**

| #  | Task                                             | Status |
| -- | ------------------------------------------------ | ------ |
| 1  | Always lock computer when away (Win + L)         | ☐      |
| 2  | Don’t let anyone tailgate into secure zones      | ☐      |
| 3  | Secure confidential papers and devices           | ☐      |
| 4  | Shred unused confidential documents              | ☐      |
| 5  | Never write down or share passwords              | ☐      |
| 6  | Keep ID badge visible and safe                   | ☐      |
| 7  | Report lost/stolen devices immediately           | ☐      |
| 8  | Use company-approved USBs only                   | ☐      |
| 9  | Escort all visitors; log entries and exits       | ☐      |
| 10 | Keep meeting rooms locked after use              | ☐      |
| 11 | Don’t connect personal USBs or hard drives       | ☐      |
| 12 | Report suspicious behaviors quietly              | ☐      |
| 13 | Don’t discuss sensitive data in public areas     | ☐      |
| 14 | Always follow offboarding access removal process | ☐      |
| 15 | Follow Clean Desk Policy every day               | ☐      |

---

## 🎯 **Outcome**

✅ Stronger protection against **internal and physical threats.**
✅ Reduced data leaks and misuse from employees or contractors.
✅ Awareness of safe workplace habits — *security becomes part of daily behavior.*
✅ Culture shift: everyone becomes **a part of the security team.**

---
