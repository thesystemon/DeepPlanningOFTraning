# 📘 Chapter 3 — Finance & Accounting Security

---

## 🧠 Learning Objectives

By the end of this session, Finance & Accounts personnel will:
✅ Understand cyber threats targeting financial systems and payments.
✅ Identify fake invoices, phishing emails, and payment diversion scams.
✅ Learn secure invoice verification and vendor validation methods.
✅ Apply safe practices for online payments, reimbursements, and payroll transfers.
✅ Know how to report and prevent Business Email Compromise (BEC).
✅ Build a zero-trust, verification-first mindset for all financial transactions.

---

## 📚 Slide / PDF Content — In Depth

---

### **Slide 1 — “Cybercriminals Love Finance Teams”**

> “Attackers follow the money — and Finance holds the key to it.”

Finance departments are the **#1 target** for Business Email Compromise (BEC) and invoice scams globally.

💰 **Why?**

* Direct access to money flows
* Access to vendor, salary, and bank accounts
* Regular communication with external vendors and clients

🧩 **Example Case:**
In 2024, a manufacturing company lost ₹1.7 crore after accounts staff paid a fake invoice that looked 99% identical to a real vendor mail — only the bank account number was changed.

📊 83% of financial frauds start with a phishing email (FBI IC3 Report, 2024).

---

### **Slide 2 — Common Threats Targeting Finance Teams**

| Threat                              | Description                                            | Example                                                                                                        |
| ----------------------------------- | ------------------------------------------------------ | -------------------------------------------------------------------------------------------------------------- |
| **Invoice Fraud**                   | Attackers send fake invoices using spoofed email IDs   | “[payment@vend0r.com](mailto:payment@vend0r.com)” instead of “[payment@vendor.com](mailto:payment@vendor.com)” |
| **Payment Diversion Scam**          | Vendor bank account details replaced by attacker’s     | “Please update our bank details urgently”                                                                      |
| **Business Email Compromise (BEC)** | CEO/CFO spoof emails requesting urgent payment         | “Transfer ₹10L immediately for audit”                                                                          |
| **Phishing / Smishing**             | Fake links to payment portals                          | “Click to verify your account”                                                                                 |
| **Payroll Fraud**                   | Employee salary diverted to hacker-controlled accounts | Change request via fake HR email                                                                               |

🧩 **Tip:** Always verify payment requests via a **second channel (phone or meeting)** before action.

---

### **Slide 3 — How Invoice & Payment Fraud Happens**

1️⃣ Attacker compromises or spoofs a vendor’s email.
2️⃣ Sends a fake invoice or payment request with changed account details.
3️⃣ Uses “urgent” tone: *“Payment pending! Late fees apply!”*
4️⃣ Finance staff pays to wrong account → money gone.

💣 Once the payment is made, reversal is almost impossible.

🧩 **Live Example:**

> Subject: *Urgent Invoice #4789 Due Today*
> “Please process payment of ₹4,75,000 to new account number — we’ve migrated banks.”

---

### **Slide 4 — How to Spot a Fake Invoice / Email**

| Red Flag                    | Description                            |
| --------------------------- | -------------------------------------- |
| ✉️ **Email mismatch**       | `@vend0r.com` instead of `@vendor.com` |
| 📁 **Unusual file type**    | `.html`, `.exe`, `.zip` attachments    |
| 💸 **Changed bank details** | New IFSC / Account Number              |
| ⏰ **Urgency pressure**      | “Pay today or late fee applies!”       |
| 🗣️ **Unverified sender**   | Not part of official vendor list       |
| 🧾 **Inconsistent format**  | Old logo, grammar errors, wrong GST    |

🧩 Activity: Show 2 real invoices — one legitimate, one fake — and ask participants to spot 5 red flags.

---

### **Slide 5 — Business Email Compromise (BEC) Defense**

| Attack Type            | Example                                                                            | Defense                              |
| ---------------------- | ---------------------------------------------------------------------------------- | ------------------------------------ |
| **CEO Fraud**          | Fake mail from “CEO” demanding urgent transfer                                     | Verify via phone / Teams             |
| **Vendor Spoofing**    | Looks like “[vendorname.invoices@gmail.com](mailto:vendorname.invoices@gmail.com)” | Use company directory to confirm     |
| **Mailbox Compromise** | Attacker reads past invoice chains                                                 | Enable MFA on all accounts           |
| **Payment Diversion**  | Bank details swapped silently                                                      | Confirm details before every payment |

🧩 **Golden Rule:**

> “No transaction without voice verification.”

---

### **Slide 6 — Secure Payment & Accounting Practices**

✔ Use **MFA (Multi-Factor Authentication)** on all finance portals (ERP, SAP, Tally, ZohoBooks).
✔ Maintain **dual authorization** for all payments above ₹50,000.
✔ Never process payments based on **email-only instructions**.
✔ Verify vendor bank account changes with **phone confirmation** to official contacts.
✔ Keep payroll and finance systems **isolated from internet browsing**.
✔ Don’t reuse finance passwords on personal accounts.

---

### **Slide 7 — Cloud, ERP & Email Security for Finance Teams**

| Area                  | Secure Practice                                  |
| --------------------- | ------------------------------------------------ |
| **ERP Access**        | Use VPN or SSO; never login via public Wi-Fi.    |
| **Email Security**    | Use official domain, enable SPF/DKIM/DMARC.      |
| **Data Sharing**      | Use encrypted Excel / PDF with password.         |
| **Backup & Recovery** | Daily backup of financial data to secure drives. |
| **Remote Work**       | VPN mandatory, disable auto-forward in email.    |

---

### **Slide 8 — Payroll & Salary Security**

| Risk                      | Example                                  | Defense                         |
| ------------------------- | ---------------------------------------- | ------------------------------- |
| Fake HR Email             | “Change employee salary account details” | Verify with HR directly         |
| Insider Theft             | Payroll admin copies employee PANs       | Access control & logging        |
| Salary Data Leak          | Spreadsheet shared externally            | Encrypt or use HRMS access only |
| Payroll Portal Compromise | Weak credentials                         | MFA + strong password policy    |

🧩 Tip: Salary slips are confidential — never send via Gmail or WhatsApp.

---

### **Slide 9 — Finance Security Checklist**

# | Task | Status

--|------|--------
1 | Verify all vendor bank changes via phone | ☐
2 | Enable MFA on finance and ERP logins | ☐
3 | Never approve payment via email alone | ☐
4 | Keep finance PCs isolated from casual browsing | ☐
5 | Encrypt financial files before sharing | ☐
6 | Conduct monthly vendor data verification | ☐
7 | Review access logs of finance systems weekly | ☐
8 | Avoid using public Wi-Fi for online payments | ☐
9 | Use official invoice templates only | ☐
10 | Report suspicious payment requests immediately | ☐

---

### **Slide 10 — Key Takeaways**

✅ Finance teams are prime targets — vigilance is your firewall.
✅ Always **verify bank changes via a call or vendor portal**.
✅ Never rush payments based on urgency or “CEO requests.”
✅ Protect login credentials — enable MFA everywhere.
✅ Treat all invoices as *potential phishing attempts* until verified.
✅ Build a “4-eye rule” — two people must approve every payment.

> “Trust your process, not your inbox.” 💰

---

## 🧩 Interactive Activities

| Activity                       | Description                                       |
| ------------------------------ | ------------------------------------------------- |
| **Fake Invoice Drill**         | Identify red flags in sample invoices.            |
| **BEC Role Play**              | Simulate “fake CEO” urgent payment request.       |
| **Dual Verification Exercise** | Practice calling vendors before payment approval. |
| **Finance Security Quiz**      | Test awareness with realistic finance scenarios.  |

---

## 🧰 Recommended Tools for Finance Security

| Tool                                 | Purpose                              | Platform |
| ------------------------------------ | ------------------------------------ | -------- |
| **VirusTotal / URLScan.io**          | Check suspicious invoice attachments | Web      |
| **DMARC Analyzer / EasyDMARC**       | Detect spoofed finance emails        | SaaS     |
| **TallyVault / ZohoBooks Shield**    | Encrypt accounting data              | ERP      |
| **Microsoft Defender / Bitdefender** | Endpoint protection                  | Windows  |
| **GoPhish / KnowBe4**                | Simulate invoice phishing tests      | SaaS     |
| **DocuSign / Adobe Sign**            | Secure invoice and approval workflow | Web      |
Would you like me to now create this **as a full visual training deck (with icons, storytelling slides, case visuals & trainer notes)** — ready for client presentation or internal training use?

---

## 🧮 15 MCQs — Finance & Accounting Security

**Q1.** Why are finance teams the top target for attackers?
A. They handle confidential HR data
B. They control money flow and payments
C. They use old computers
D. They have internet access
✅ **Answer: B**

**Q2.** What’s the first sign of an invoice fraud attempt?
A. Vendor name change
B. Bank detail update request via email
C. File size large
D. Payment amount less
✅ **Answer: B**

**Q3.** What is Business Email Compromise (BEC)?
A. Email password reset issue
B. Fake emails to manipulate financial transactions
C. Hardware attack
D. Server downtime
✅ **Answer: B**

**Q4.** The safest way to confirm a vendor bank change is:
A. Call official vendor contact directly
B. Reply to email
C. Trust attached PDF
D. Wait 2 days
✅ **Answer: A**

**Q5.** What is the “4-eye rule”?
A. Two-person verification for all critical payments
B. Reading emails carefully
C. Double-checking invoices visually
D. Video meeting approval
✅ **Answer: A**

**Q6.** What should be done when receiving a payment request from CEO’s email?
A. Process immediately
B. Verify in person or by phone
C. Reply “OK”
D. Ignore
✅ **Answer: B**

**Q7.** What is the most common attachment type in finance phishing?
A. .exe or .zip
B. .png
C. .mp4
D. .txt
✅ **Answer: A**

**Q8.** Which protocol prevents email spoofing?
A. FTP
B. SPF/DKIM/DMARC
C. HTTP
D. DNS
✅ **Answer: B**

**Q9.** What should you do if you paid to a fake account?
A. Report immediately to bank & IT/security
B. Delete evidence
C. Do nothing
D. Inform vendor only
✅ **Answer: A**

**Q10.** Dual authorization helps prevent:
A. Email overload
B. Unauthorized fund transfers
C. VPN failure
D. Backup loss
✅ **Answer: B**

**Q11.** Which is *not* a safe payment practice?
A. MFA on ERP
B. Direct payment from personal account
C. Two-step approval
D. Secure VPN
✅ **Answer: B**

**Q12.** What should finance teams do before opening invoice attachments?
A. Scan with VirusTotal or antivirus
B. Open directly
C. Forward to colleague
D. Upload to cloud
✅ **Answer: A**

**Q13.** Which of these is a form of social engineering?
A. Fake urgent email from vendor
B. Server crash
C. Password expiry notice
D. System update alert
✅ **Answer: A**

**Q14.** What’s the best password practice for finance users?
A. Use complex unique passwords with MFA
B. Share password with assistant
C. Use same password for ERP and email
D. Keep password written on paper
✅ **Answer: A**

**Q15.** What is the correct response to “update vendor account urgently”?
A. Verify by calling the vendor
B. Approve directly
C. Delay one week
D. Forward to all
✅ **Answer: A**

✅ **Answer Key:** 1B, 2B, 3B, 4A, 5A, 6B, 7A, 8B, 9A, 10B, 11B, 12A, 13A, 14A, 15A

---

## 🎯 Outcomes

✅ Finance teams can identify fake invoices & payment diversion scams.
✅ Payments are verified through dual authorization and vendor validation.
✅ Reduced financial loss and phishing incidents.
✅ Increased compliance with internal audit and fraud control frameworks.
✅ Finance evolves from “target zone” to **secure transaction guardian.**

> “Cybercriminals steal trust before they steal money — verify everything.” 💼

---

