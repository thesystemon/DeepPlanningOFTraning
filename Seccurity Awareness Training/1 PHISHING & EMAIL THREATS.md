# 📘 CHAPTER 1 — PHISHING & EMAIL THREATS (DEEP, CLIENT-READY)

## ✳️ Module overview (one-line)

Teach employees to detect, avoid, and report phishing attempts — turning them into an active line of defense.

---

## 🧠 Learning objectives (what learners should be able to do)

* Explain what phishing is and why it’s dangerous.
* Identify common signs of phishing in emails, SMS, and calls.
* Safely analyze suspicious links and attachments at a basic level.
* Report suspicious messages through the organization’s defined channel.
* Follow immediate steps if they accidentally clicked or submitted information.

---

## 📚 Slide / PDF content — detailed breakdown (use these as slides)

### Slide 1 — Title / Hook

**PHISHING & EMAIL THREATS**
Subtitle: “How attackers trick people — and exactly what you should do.”

---

### Slide 2 — What is phishing?

* **Definition:** Phishing is a type of social engineering where attackers send fake messages (email, SMS, or voice) designed to trick you into giving away sensitive information (passwords, bank details), clicking malicious links, or opening harmful attachments.
* **Why it works:** Attackers exploit trust, urgency, fear, curiosity, or authority. Technical controls help, but people are often the weakest link.

---

### Slide 3 — Real-world consequences

* Credential theft → account takeover.
* Malware/ransomware infection from malicious attachments or downloads.
* Data breaches → customer / company data exposed.
* Financial fraud (wire transfer scams) and business email compromise (BEC).
* Reputational damage and regulatory fines.

---

### Slide 4 — Common signs of phishing (visual checklist)

* **Urgent or threatening language:** “Your account will be suspended.”
* **Mismatched sender:** visible name says “HR”; actual email is `hr-notify@xyz-secure.com`.
* **Spelling/grammar errors** and awkward phrasing.
* **Unexpected attachments** (ZIP, EXE, macro-enabled Office files).
* **Shortened or odd links** (bit.ly, tinyurl pointing to external domains).
* **Generic greetings** (“Dear Customer” vs your real name).
* **Requests for credentials, OTPs, or sensitive data** via email.

---

### Slide 5 — Types of phishing (definitions + examples)

* **Email phishing:** mass emails pretending to be banks, vendors, or services.
* **Spear phishing:** targeted attacks using personal info (job role, manager name).
* **Business Email Compromise (BEC):** attacker spoofs or compromises exec email to request wire transfers or invoices.
* **Smishing:** phishing via SMS (short message).
* **Vishing:** voice call scams (deepfake voices are a rising risk).
* **Quishing:** QR-code based phishing (scan QR → malicious URL).

---

### Slide 6 — Anatomy of a typical phishing email (visual)

* From: display name / real-from header mismatch
* Subject: urgent CTA
* Pre-header: short teaser text
* Body: short paragraph asking for action
* Link/Button: disguised URL
* Attachment: suspicious file
* Footer: fake company signature/logo

*(Show screenshot examples — sanitized or recreated safe examples; never show live malicious content.)*

---

### Slide 7 — How to inspect links safely

* **Hover to preview**: mouse-over the link to see the actual destination (do not click).
* **Look for domain typos**: `micr0soft.com` vs `microsoft.com`.
* **If the domain looks odd, do not click.**
* **Use link checkers** if unsure (internal sandbox, VirusTotal for admins).
* For mobile: long-press link to preview destination (or copy link and paste into a safe notepad first — but only admins should use external scanners).

---

### Slide 8 — Attachments: what to avoid

* **Never open** `.exe`, `.scr`, `.bat`, `.msi`, or macro-enabled `.docm/.xlsm` from unknown senders.
* **Zip files** sometimes contain malicious EXEs — treat with caution.
* If attachment is expected, **confirm by alternate channel** (call the sender’s known number).
* Company policy: attachments should be scanned by endpoint protection and sandboxes.

---

### Slide 9 — Social engineering cues (psychology)

* **Urgency:** “Act now or lose access.”
* **Authority:** “CEO needs this wire transfer.”
* **Scarcity/curiosity:** “You have one unread invoice.”
* **Reciprocity/trust:** attacker references internal info to sound legit.

---

### Slide 10 — Reporting procedure (clear, step-by-step)

**Always follow the organizational reporting workflow. Example:**

1. Do NOT click any more links in the message.
2. Use your email client’s “Report Phishing” / “Report Message” button (Outlook → Report Message add-in / Gmail → Report phishing).
3. Forward the message to the SOC inbox: `phish@company.com` (or the client’s defined address) **with subject: “Suspected Phish – [Short note]”**.
4. If you entered credentials or clicked a link that requested credentials → immediately notify IT/SOC and change passwords (start with MFA method) and follow incident response instructions.
5. If it's wire-transfer related or CFO/CEO impersonation, **call your manager and security immediately** (do not email).

*(Include screenshots of how to use Outlook/Gmail report buttons — safe instructional images.)*

---

### Slide 11 — If you clicked / submitted information — immediate steps

1. Disconnect from network (if instructed by IT).
2. Inform IT/SOC immediately (phone or escalation channel).
3. Change password(s) on affected systems — use a different device if possible.
4. Revoke active sessions (e.g., sign out of all devices).
5. If MFA token was shared, revoke/reset MFA or re-register device.
6. Watch for suspicious account activity and follow up investigation.

---

### Slide 12 — Business Email Compromise (BEC) — red flags & control

* **Red flags:** last-minute invoice changes, new payment instructions, pressure to keep the request secret.
* **Controls:** always verify payment changes via known phone number, dual-approval workflows for high-value transfers, whitelist vendor invoices, and use positive pay for bank transfers.

---

### Slide 13 — Practical detection tools for users (what we provide)

* Outlook “Report Message” add-in configured.
* Simple one-click “Report” forwarding rule to SOC.
* Department champions trained to triage reported emails.
* Quick-reference PDF: “What to do if you receive a suspicious email.”

---

### Slide 14 — Hands-on activities (delivery plan)

* **Live demo (trainer):** open safe example emails, show link hover, show header inspection, show how to report.
* **Phishing simulation:** run a controlled GoPhish campaign (with client permission).
* **Group exercise:** show 6 email screenshots (safe examples) and ask teams to mark which are phishing.
* **Quiz:** 5–15 MCQs (use provided set below).
* **Roleplay:** a fake vishing call scenario for a small group.

---

### Slide 15 — GoPhish campaign blueprint (safe, non-malicious)

**Goal:** Measure click rate and reporting behavior, teach via follow-up.
**High-level steps (trainer-run):**

* Obtain written permission from client + define scope (which departments/emails).
* Prepare a **harmless landing page** that captures email only for learning (no passwords) and displays an educational message: “This was a safe phishing test — here’s what you should have noticed.”
* Create 2–3 realistic templates (e.g., Password Expiry, HR Document Request, Delivery Notification). Avoid sensitive lures (bank/finance wire instructions) unless client approves.
* Schedule campaign for a non-critical time.
* After campaign: aggregate metrics (open %, click %, submitted info %, reported %) and run immediate remediation emails + short micro-training for those who clicked.
* Share anonymized results with management and recommendations.

> **Ethics:** Never capture real credentials; never use malicious payloads; always debrief participants.

---

### Slide 16 — Measurement & Reporting (KPIs)

* **Phish-prone % (click rate):** % who clicked the test link.
* **Report rate:** % who used the report button or forwarded to SOC.
* **Credential submission rate:** % who submitted any data (trainer must ensure no real credentials are requested).
* **Trend:** phish-prone % over time (before vs after training).
* **Departmental breakdown:** Which teams need focused training.

---

### Slide 17 — Trainer checklist (ready to deliver)

* Get client permission & scope signed.
* Prepare sanitized example emails and screenshots.
* Configure Outlook/Gmail report add-in and SOC mailbox.
* Create GoPhish templates + educational landing page.
* Prepare slides, demo machine (isolated), and quizzes.
* Prepare follow-up learning for clicked users (5–10 min micro-module).

---

### Slide 18 — One-page employee cheat-sheet (handout)

* **Top 5 Signs of Phishing** (brief bullets).
* **Quick actions:** Don’t click → Report → Forward to SOC → If you shared credentials, call IT.
* **Reporting contact:** [phish@company.com](mailto:phish@company.com) / ext. 1234 / security hotline.

---

## 📈 Delivery / Activity — session plan (60-minute example)

* 0–5 min: Intro & Hook (stories/statistics).
* 5–20 min: What is phishing + types + examples + demo link hover.
* 20–30 min: Anatomy of a phishing email + header basics.
* 30–40 min: Live demo — reporting steps (Outlook/Gmail).
* 40–50 min: Group exercise: identify phishing in screenshots.
* 50–55 min: Quiz (5–10 MCQs) — Google Forms.
* 55–60 min: Wrap-up & next steps (phishing simulation planned, reporting channels).

---

## 🧩 Outcome

After this module employees will be able to: spot common phishing indicators, safely report suspicious messages per company policy, and follow immediate steps if they clicked — leading to a measurable reduction in click rates over time.

---

## ⚠️ Safety & Legal Notes (must include in client proposal)

* Obtain **written approval** from client before any simulation.
* Never ask for real passwords or PII in landing pages.
* Avoid sensitive lures (e.g., payroll wire transfer) unless client explicitly approves.
* Provide pre- and post-simulation communication to avoid panic.

---

## ✅ Trainer Resources to Attach (deliverable files)

* Slide deck (editable PPT) — uses the slides above.
* One-page cheat-sheet PDF for employees.
* GoPhish templates (text only) — three non-sensitive email templates.
* Google Forms quiz (MCQs) — ready to import.
* Reporting dashboard template (Google Sheets) — KPI tracker.

---

# 🎯 15 MCQs (Use in Google Forms / MS Forms)

Below are 15 multiple-choice questions with correct answers and short explanations. Use these verbatim in your quiz.

---

### Q1. What is phishing?

A. A software patch
B. A method to trick people into revealing sensitive information
C. A type of firewall
D. An antivirus update
**Answer:** B
**Explanation:** Phishing is social engineering used to trick people into giving up sensitive information or performing unsafe actions.

---

### Q2. Which of these is a common sign of a phishing email?

A. Email from your manager with correct email address and internal references
B. An email with perfect grammar and internal links
C. Urgent language asking you to “act now” and unknown sender address
D. A calendar invite from your team
**Answer:** C
**Explanation:** Urgency and unknown senders are common phishing indicators.

---

### Q3. When you hover over a link in an email, what are you trying to find?

A. The color of the link
B. The real destination domain (URL)
C. The font size
D. The sender’s job title
**Answer:** B
**Explanation:** Hovering reveals the actual URL destination so you can spot suspicious domains.

---

### Q4. Which attachment type is most dangerous to open from an unknown sender?

A. .txt
B. .jpg
C. .exe
D. .pdf
**Answer:** C
**Explanation:** Executable files (.exe) can directly run code and are high risk.

---

### Q5. Smishing refers to phishing via:

A. Email
B. Postal mail
C. SMS / text messages
D. Social media posts
**Answer:** C
**Explanation:** Smishing is phishing delivered by SMS messages.

---

### Q6. If you receive an unexpected file from a known colleague, what’s the safest first step?

A. Open it immediately
B. Reply asking for more files
C. Contact the colleague by phone or internal chat to verify they sent it
D. Forward it to everyone in the team
**Answer:** C
**Explanation:** Verify via an alternate channel before opening unexpected attachments.

---

### Q7. Which of these is a sign of Business Email Compromise (BEC)?

A. A routine meeting invite
B. A request to change bank payment details, sent urgently by an executive’s email that has odd tone
C. A software update notification from IT
D. An email newsletter
**Answer:** B
**Explanation:** BEC often involves urgent payment changes from lookalike or compromised exec emails.

---

### Q8. What should you do if you accidentally enter your password into a suspicious site?

A. Ignore it
B. Change your password immediately and notify IT/SOC
C. Try the password again on other sites
D. Wait 48 hours to see if anything happens
**Answer:** B
**Explanation:** Immediately change the password and inform security to limit damage.

---

### Q9. Which of these increases protection against phishing even if your password is stolen?

A. Using the same password everywhere
B. Disabling browser updates
C. Enabling Multi-Factor Authentication (MFA)
D. Sharing your password with IT
**Answer:** C
**Explanation:** MFA adds an extra layer of verification, reducing risk from stolen passwords.

---

### Q10. Which is the best way to report a suspicious email in Outlook?

A. Delete it quietly
B. Click links in it to check where they go
C. Use the “Report Message” add-in or forward to [phish@company.com](mailto:phish@company.com)
D. Print it and file in physical records
**Answer:** C
**Explanation:** Reporting via the built-in tool or to SOC allows proper investigation and blocking.

---

### Q11. What is spear phishing?

A. A mass email sent to everyone
B. A targeted phishing attack that uses personal information about the victim
C. A phishing email with no links
D. A phishing attack that only affects mobile phones
**Answer:** B
**Explanation:** Spear phishing targets specific individuals using personal or organizational info.

---

### Q12. Why should you avoid clicking shortened URLs (like bit.ly) in suspicious messages?

A. They are always safe
B. They hide the real destination and can point to malicious sites
C. They load faster
D. They are used only for images
**Answer:** B
**Explanation:** Short links conceal the destination, making it easier to hide malicious sites.

---

### Q13. Which of these behaviors is safest when you get an urgent payment request by email?

A. Transfer money immediately to avoid delays
B. Verify the request via a separate channel (phone call to known number) before acting
C. Reply “OK” to the email to confirm
D. Forward to the entire department for confirmation
**Answer:** B
**Explanation:** Verifying via a known phone number reduces risk of BEC scams.

---

### Q14. A footer with a company logo guarantees the email is legitimate. True or False?

A. True
B. False
**Answer:** B (False)
**Explanation:** Logos can be copied; always verify sender domain and other indicators.

---

### Q15. Which of the following is an appropriate post-reporting action by the SOC?

A. Ignore the report
B. Block the sender domain if malicious and share warning to employees
C. Publicly name the employee who clicked the email
D. Delete employee mailboxes
**Answer:** B
**Explanation:** SOC should mitigate threat (block, quarantine) and inform staff; never shame employees publicly.

---

## ✅ Answer key (for quick copy/paste)

1:B, 2:C, 3:B, 4:C, 5:C, 6:C, 7:B, 8:B, 9:C, 10:C, 11:B, 12:B, 13:B, 14:B, 15:B

---

## 🛠️ Trainer notes for running the quiz

* Use Google Forms/MS Forms; set one correct answer per question for auto-grading.
* After quiz submission, show correct answers + short explanation.
* For those who score below threshold (e.g., <70%), assign a 10-min refresher module.

---

## 🔁 Post-training follow-up (30–90 days)

* Run a GoPhish simulation and compare click/report rates pre/post training.
* Share anonymized results and a 1-page executive summary with client: completion %, quiz avg, phish-prone % before vs after.
* Re-train departments with high click rates.

---

## 📝 Sample GoPhish non-sensitive email templates (text-only) — trainer may adapt

**Template A – Password Expiry (educational only)**
*Subject:* Action required: Update your company password
*Body:* Hello [FirstName], our systems show your password expires today. Please click the link below to confirm your account details. — **Note:** Landing page must not ask for actual passwords; instead show educational content and ask user to acknowledge they saw the training.

**Template B – HR Document (safe)**
*Subject:* Updated HR policy: Please review and acknowledge
*Body:* Hello [FirstName], please review the attached updated HR policy. Click here to view the document. — Landing page explains the test.

**Template C – Delivery Notice (safe)**
*Subject:* Your package delivery requires confirmation
*Body:* Hello [FirstName], we attempted to deliver a package. Please click here to confirm delivery details. — Landing page educational.

> Important: Always include in landing page: “This was a simulated phishing test. No action required. Here are 3 tips to spot phishing.” Do not request credentials.

---

## 📊 Metrics & reporting template (quick)

* Total recipients: X
* Open rate: Y%
* Click rate: Z%
* Report rate: R%
* Clicks by department (table)
* Recommended next steps (top 3)

---

## Final quick checklist for client delivery

* [ ] Client signs phishing simulation consent & scope doc.
* [ ] Configure reporting address (`phish@client.com`) and Outlook button.
* [ ] Trainer prepares sanitized demo emails and slides.
* [ ] Run live training session + quiz.
* [ ] Schedule GoPhish simulation (if agreed).
* [ ] Send remediation micro-training to clicked users.
* [ ] Deliver KPI report after simulation and monthly follow-up.

---


