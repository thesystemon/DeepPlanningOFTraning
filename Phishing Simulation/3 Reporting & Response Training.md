# 📘 Chapter 3 — Reporting & Response Training

---

## 🧠 Learning Objectives

By the end of this session, employees will be able to:

✅ Report suspicious emails, messages, or files using the correct channels.
✅ Understand **why** timely reporting is critical for incident containment.
✅ Learn how the **IT/SOC (Security Operations Center)** responds to reported threats.
✅ Follow escalation and documentation steps confidently.
✅ Build a proactive mindset — **“See Something, Say Something.”**

---

## 🧩 Slide 1 — “The Power of the First Reporter”

> “The fastest click can start an attack. The fastest report can stop it.”

In cybersecurity, **speed matters more than perfection**.
Every minute a phishing email stays unreported increases the chance that others might fall for it.

📊 **Fact:**
Organizations with strong internal reporting see up to **70% fewer successful phishing incidents** (source: Verizon DBIR).

💡 **Trainer Story Example:**
In one company, an employee reported a suspicious invoice within 5 minutes. IT blocked 48 similar phishing emails in other inboxes — preventing a company-wide compromise.
That one report **saved the company’s finance system**.

---

## 🧩 Slide 2 — Why Reporting Matters

Reporting isn’t just about following rules — it’s about **protecting people and systems**.

### 🎯 Key Benefits of Immediate Reporting:

* **Stops the Spread:** IT can block similar emails across all accounts.
* **Reduces Damage:** Early action prevents data leaks or malware spread.
* **Improves Defense:** Every report helps security teams update filters and train smarter AI-based detectors.
* **Builds Security Culture:** Reporting becomes second nature, like wearing a seatbelt — automatic and safe.

💬 **Example:**
If an employee clicks a malicious link and doesn’t report it, the attacker may use that one compromised account to send more phishing emails internally — multiplying damage.

---

## 🧩 Slide 3 — Reporting Steps (Deep Breakdown)

| Step                                     | Action                                                                                 | Why It’s Important                                     |
| ---------------------------------------- | -------------------------------------------------------------------------------------- | ------------------------------------------------------ |
| **1️⃣ Don’t Click or Reply**             | Never interact with suspicious content.                                                | Prevents malware installation or credential theft.     |
| **2️⃣ Report the Message**               | Use the **“Report Message” add-in** in Outlook or Gmail.                               | Instantly alerts the Security Operations Center (SOC). |
| **3️⃣ Forward Manually (if needed)**     | Send to **[security@company.com](mailto:security@company.com)** or official SOC email. | Ensures your report is tracked and analyzed.           |
| **4️⃣ Document Briefly**                 | Add details like sender address, time received, subject, and any action taken.         | Helps IT investigate efficiently.                      |
| **5️⃣ Delete or Quarantine the Message** | Only after reporting.                                                                  | Prevents accidental clicks by others.                  |

💡 **Trainer Tip:**
Demonstrate this process live.
Show employees exactly where the **“Report Phishing”** button is in their mail client (Outlook, Gmail, Teams, etc.).

---

## 🧩 Slide 4 — Escalation Path: Who Handles What

When you report, your message **activates a response chain** within the organization.

**1️⃣ Employee (You):** Identify and report suspicious activity.
**2️⃣ IT Helpdesk:** Acknowledges your report and performs initial triage.
**3️⃣ SOC Team:** Analyzes headers, URLs, and attachments for threat intelligence.
**4️⃣ Security Manager:** Assesses business impact, coordinates response.
**5️⃣ Incident Response Team (IRT):** Containment, mitigation, and post-incident report.

### 🔄 Example Workflow:

```
You → security@company.com → IT Helpdesk → SOC → IRT
```

💡 **Trainer Tip:**
Show this chain visually using a flowchart. Helps employees understand **how their one report can trigger a coordinated defense**.

---

## 🧩 Slide 5 — IT/SOC Response Process

Once a report reaches the Security Operations Center, the following **technical workflow** begins:

| Phase                    | SOC Action                                             | Example                                |
| ------------------------ | ------------------------------------------------------ | -------------------------------------- |
| **1️⃣ Collect**          | SOC receives reported email via tool or inbox.         | Outlook “Report Phish” alert received. |
| **2️⃣ Analyze**          | Header analysis, domain check, sandboxing attachments. | Detects malicious URL.                 |
| **3️⃣ Contain**          | Block domain/company-wide, isolate infected machines.  | URL added to blocklist.                |
| **4️⃣ Eradicate**        | Remove malicious artifacts or compromised credentials. | Reset user passwords.                  |
| **5️⃣ Recover & Review** | System restored, lessons learned documented.           | Policy updated, training adjusted.     |

🔐 **Key Insight:**
The SOC can’t act unless users **report incidents promptly** — the human layer is the **first alert sensor**.

---

## 🧩 Slide 6 — Do’s and Don’ts When Reporting

### ✅ Do’s:

* Use **official reporting tools** (no screenshots on WhatsApp).
* Report even if you’re **unsure** — false alarms are okay.
* Include **full headers or message trace** if possible.
* Report **accidental clicks** immediately — don’t hide mistakes.

### ❌ Don’ts:

* Don’t forward phishing emails to colleagues.
* Don’t delete before reporting.
* Don’t attempt to “fix” or “analyze” the message yourself.
* Don’t ignore small or harmless-looking emails — many big attacks start small.

💡 **Trainer Example:**
Simulate a “mistake reporting” scenario. Show that even if an employee clicked a link, **reporting quickly can limit damage** — not reporting can make it worse.

---

## 🧩 Slide 7 — Common Reporting Mistakes

| Mistake                              | Why It’s Risky                      | Better Practice                     |
| ------------------------------------ | ----------------------------------- | ----------------------------------- |
| Waiting until the next day to report | Attack spreads overnight            | Report immediately                  |
| Reporting through chat or text       | Not traceable                       | Use official email/reporting add-in |
| Deleting message before reporting    | Evidence lost                       | Report first, delete later          |
| Forwarding the phishing email        | Increases risk of accidental clicks | Use “Report Message” tool           |

💡 **Trainer Tip:**
Show before-after comparison: what happens when a phishing message is reported instantly vs ignored for 4 hours. (Visual timeline helps reinforce urgency.)

---

## 🧩 Slide 8 — Building a Reporting Culture

> “Security is not just a department — it’s everyone’s responsibility.”

### 🔁 Reinforcement Habits:

* Regular **phishing simulations** keep awareness sharp.
* **Recognition programs** (points or badges) reward active reporters.
* **Transparency** in incident handling builds employee trust.
* **Micro-learning tips** reinforce behavior weekly.

💬 Example:
A “Report of the Month” shoutout during internal meetings boosts engagement and motivates others to act quickly next time.

---

## 🧩 Slide 9 — Post-Reporting Actions (After You Report)

After submitting your report:

✅ **Don’t panic.** SOC will handle the technical side.
✅ **Wait for confirmation** from IT/SOC if additional steps are required.
✅ If you **clicked a link or entered credentials**, immediately:

* Disconnect from the network.
* Inform IT to reset passwords and scan system.
  ✅ Reflect and learn — what tricked you? So next time, you’ll spot it faster.

💡 **Trainer Exercise:**
Role-play:

* One employee reports a phishing email.
* SOC team explains next steps.
* Debrief as a group — discuss what went well and what could improve.

---

## 🧩 Slide 10 — Continuous Response Improvement

Incident reporting is not a one-time event — it’s a **loop of learning**.

### 🔄 Continuous Improvement Cycle:

1️⃣ **Report** suspicious item.
2️⃣ **Analyze** and contain by SOC.
3️⃣ **Share lessons learned.**
4️⃣ **Update training & filters.**
5️⃣ **Simulate again** to measure improvement.

This creates an **ever-evolving human firewall** that adapts faster than attackers.

---

## 🧮 10 Sample MCQs — Reporting & Response Training

1️⃣ What is the **first action** when you receive a suspicious message?
A. Click link to verify
B. Report without interacting ✅
C. Delete immediately
D. Ask your colleague

2️⃣ Where should you report phishing emails?
A. Personal email
B. [security@company.com](mailto:security@company.com) ✅
C. WhatsApp
D. Public post

3️⃣ Why should you NOT forward phishing emails?
A. Wastes inbox space
B. Can spread the threat ✅
C. Makes IT angry
D. Is illegal

4️⃣ What tool helps in reporting phishing directly?
A. Outlook “Report Message” add-in ✅
B. Word Processor
C. Screenshot app
D. PDF viewer

5️⃣ Who investigates your report after IT Helpdesk?
A. HR Team
B. SOC Team ✅
C. Marketing
D. Finance

6️⃣ Why should you include sender and subject in your report?
A. Helps SOC identify attack pattern ✅
B. Looks professional
C. Optional detail
D. Saves storage

7️⃣ What should you do after reporting and deleting the message?
A. Wait for SOC confirmation ✅
B. Ignore
C. Reopen message
D. Post online

8️⃣ Why are delayed reports dangerous?
A. Attack may spread ✅
B. Email storage fills up
C. SOC gets bored
D. No reason

9️⃣ What’s the best mindset for reporting?
A. “I might be wrong — I’ll still report.” ✅
B. “Only IT should report.”
C. “Wait until multiple people complain.”
D. “Ignore minor threats.”

10️⃣ What’s the final step in the response cycle?
A. Report
B. Contain
C. Learn & Improve ✅
D. Delete emails

---

## ✅ Chapter 3 — Reporting & Response Checklist

| #  | Task                                                         | Status |
| -- | ------------------------------------------------------------ | ------ |
| 1  | Employees know how to report phishing via official channels  | ☐      |
| 2  | Employees understand escalation path (User → IT → SOC → IRT) | ☐      |
| 3  | Employees avoid forwarding or replying to suspicious emails  | ☐      |
| 4  | Reports are documented with sender, subject, and time        | ☐      |
| 5  | SOC processes reports with clear workflow                    | ☐      |
| 6  | Employees report accidental clicks without fear              | ☐      |
| 7  | Phishing simulations include reporting practice              | ☐      |
| 8  | Reporting metrics are tracked on dashboard                   | ☐      |
| 9  | Recognition programs encourage reporting                     | ☐      |
| 10 | Continuous learning cycle implemented                        | ☐      |

---

## 🎯 Outcomes

✅ Employees report suspicious messages instantly and accurately.
✅ SOC receives high-quality, timely data for threat analysis.
✅ Reduced infection spread and faster containment of incidents.
✅ Stronger collaboration between employees and IT/SOC.
✅ Company culture shifts from reactive to proactive security.

---


