# 📘 Chapter 2 — HR & Recruitment Team Security

---

## 🧠 Learning Objectives

By the end of this session, HR & Recruitment personnel will:
✅ Understand their responsibility in protecting candidate and employee data.
✅ Recognize phishing, social engineering, and recruitment scams targeting HR.
✅ Learn how to handle personal data (PII, resumes, ID proofs) securely.
✅ Implement secure onboarding/offboarding procedures.
✅ Identify risks in third-party recruitment portals and background verification vendors.
✅ Prevent insider data leakage or accidental exposure.

---

## 📚 Slide / PDF Content — In Depth

---

### **Slide 1 — “HR: The Human Gateway to Cybersecurity”**

> “Attackers don’t always hack systems — they hack people who have access to them.”

HR departments handle **the most sensitive data** in any organization:

* Candidate CVs, IDs, phone numbers
* Employee addresses, bank details, salary slips
* Background verification reports, medical or legal records

🧩 **Trainer Tip:** Start with a real case:
*An HR employee clicked on a fake “job applicant resume.zip” — it contained malware that spread company-wide within 10 minutes.*

📊 82% of HR professionals receive phishing emails disguised as job applications (Proofpoint, 2024).

---

### **Slide 2 — Common Threats Targeting HR Teams**

| Threat Type                  | Description                                                | Example                                             |
| ---------------------------- | ---------------------------------------------------------- | --------------------------------------------------- |
| **Phishing Resumes**         | Fake CVs containing malware attachments (.zip, .docm)      | “Resume_John.docm” installs a trojan.               |
| **Fake Job Portals**         | Imitation of Naukri/LinkedIn pages to steal HR credentials | HR logs into a clone portal.                        |
| **Social Engineering Calls** | Callers posing as candidates, vendors, or auditors         | “Can you confirm employee salary for verification?” |
| **Data Exfiltration**        | Insider copying candidate lists or payslips                | Disgruntled employee leaks data.                    |
| **Third-party Vendor Risks** | Weak security in external background agencies              | Data breach during verification.                    |

🧩 Demo: Show a “fake job application email” and highlight red flags (mismatched domains, grammar, attachment types).

---

### **Slide 3 — Data Privacy & PII (Personal Identifiable Information)**

PII = Any data that identifies a person.
HR handles massive volumes of it.

| Data Type             | Example                    | Handling Rule                      |
| --------------------- | -------------------------- | ---------------------------------- |
| **Basic PII**         | Name, phone, email         | Store only in secure HRMS.         |
| **Sensitive PII**     | PAN, Aadhaar, medical info | Encrypt and restrict access.       |
| **Financial Info**    | Salary, bank details       | Use secure transfer only.          |
| **Background Checks** | Legal/educational data     | Share with verified partners only. |

🧩 Activity: Participants identify what type of data is shown (e.g., Resume, ID proof, payslip) and classify it (Public / Internal / Confidential).

---

### **Slide 4 — Secure HR Data Handling Lifecycle**

1️⃣ **Collection:**

* Gather only necessary data during recruitment.
* Use official portals/forms (no WhatsApp/email forms).
* Get candidate consent.

2️⃣ **Storage:**

* Use secure HRMS tools (SAP SuccessFactors, BambooHR, Keka, Zoho People).
* Encrypt backups.

3️⃣ **Access & Sharing:**

* Limit access to authorized HR members only.
* Don’t email unencrypted resumes or spreadsheets.
* Use company-approved sharing tools (SharePoint, OneDrive, Nextcloud).

4️⃣ **Disposal:**

* Delete rejected candidate data as per retention policy (e.g., 6 months).
* Shred printed resumes and ID copies.

🧩 Tip: Implement a “Least Privilege” model — HR interns should not access salary data.

---

### **Slide 5 — Social Engineering Defense for HR Teams**

Common Scenarios:
⚠️ “Candidate” calls asking to confirm who handles recruitment for job openings.
⚠️ “Vendor” sends fake background verification requests.
⚠️ “Auditor” requests employee data “urgently”.

🧩 **Golden Rule:**

> “Verify first — share never.”

✔ Always verify caller identity via official contact list.
✔ Don’t share employee/candidate data over phone or SMS.
✔ Report suspicious communications to IT/Security immediately.

🎭 Activity: Role-play “imposter caller” scenario and have HR identify red flags.

---

### **Slide 6 — Secure Recruitment Process**

| Stage                    | Risk                     | Security Practice                              |
| ------------------------ | ------------------------ | ---------------------------------------------- |
| **Job Posting**          | Fake job ads by scammers | Post only on verified company domains/portals. |
| **Candidate Screening**  | Malware resumes          | Open resumes in sandbox or preview mode only.  |
| **Interview Scheduling** | Calendar invite scams    | Confirm invite links & domains.                |
| **Offer Letter Stage**   | Fake offer scams         | Use digital signature + company letterhead.    |
| **Onboarding**           | Sharing sensitive docs   | Use secure onboarding portals (encrypted).     |

🧩 Case Study: Fake recruiter scam — attackers posing as company HR collected ₹5,000 “security deposit” from candidates via Telegram.

---

### **Slide 7 — Insider Threats in HR**

| Type                   | Example                   | Prevention                               |
| ---------------------- | ------------------------- | ---------------------------------------- |
| **Malicious Insider**  | HR employee selling data  | Strict access logs & monitoring.         |
| **Negligent Insider**  | Leaving files open/shared | Enforce Clean Desk & Lock Screen policy. |
| **Accidental Insider** | Sending wrong attachment  | Double-check before emailing data.       |

🧩 Tip: Conduct periodic “Access Rights Audit” for HR folders & drives.

---

### **Slide 8 — Legal & Compliance (Simplified for HR)**

| Regulation                | Applies To                            | Key HR Impact                                         |
| ------------------------- | ------------------------------------- | ----------------------------------------------------- |
| **India DPDP Act (2023)** | Personal data of candidates/employees | Must collect only with consent & retain minimum data. |
| **GDPR (EU)**             | EU candidate data                     | Right to be forgotten; lawful processing.             |
| **ISO 27001 / SOC 2**     | Internal HR data handling             | Maintain confidentiality & audit trails.              |
| **Company Policy**        | Local data management                 | Follow HRIS security SOP.                             |

🧩 Message: “Every resume you handle is a compliance artifact.”

---

### **Slide 9 — HR Security Checklist**

# | Task | Status

--|------|--------
1 | Collect candidate data only through official forms | ☐
2 | Store resumes and IDs in secure HRMS | ☐
3 | Don’t open resumes from unknown emails | ☐
4 | Encrypt files with personal data | ☐
5 | Delete old candidate data as per policy | ☐
6 | Verify all third-party HR vendors | ☐
7 | Lock systems when leaving desk | ☐
8 | Don’t share data on WhatsApp or Gmail | ☐
9 | Verify all verification requests | ☐
10 | Report any suspected phishing attempt | ☐

---

### **Slide 10 — Key Takeaways**

✅ HR = the first and last line of defense for employee data.
✅ Verify every request before sharing personal or salary info.
✅ Store candidate data securely, delete responsibly.
✅ Don’t click or download attachments from unknown applicants.
✅ Report suspicious calls, emails, or vendors.
✅ Protecting candidate trust = protecting company reputation.

> “Every resume is data. Every data is responsibility.”

---

## 🧩 Interactive Activities

| Activity                         | Description                                                                         |
| -------------------------------- | ----------------------------------------------------------------------------------- |
| **Resume Malware Drill**         | Open fake resumes (in sandbox) and identify malicious file types (.exe, .js, .zip). |
| **Social Engineering Role Play** | Simulate a fake recruiter or vendor call.                                           |
| **Data Handling Quiz**           | 10-question quick test (Forms or Kahoot).                                           |
| **Clean Desk Challenge**         | Inspect workspace — no exposed PII allowed!                                         |

---

## 🧰 Free Tools for HR Security

| Tool                                  | Purpose                           | Platform      |
| ------------------------------------- | --------------------------------- | ------------- |
| **Google Safe Browsing / VirusTotal** | Scan attachments & links          | Web           |
| **DocuSign / Adobe Sign**             | Secure digital offers & contracts | Web           |
| **Bitwarden / 1Password**             | Password vault                    | All           |
| **Nextcloud / OneDrive**              | Secure file sharing               | Cloud         |
| **BleachBit / Eraser**                | Secure data deletion              | Windows/Linux |
| **KnowBe4 / GoPhish**                 | Phishing simulations              | SaaS          |
| **Zoom / MS Teams Verified Links**    | Secure meeting invites            | Collaboration |

---

## 🧮 15 MCQs — HR & Recruitment Team Security

**Q1.** Why is HR a top target for cyberattacks?
A. Handles large budgets
B. Handles personal and sensitive data
C. Has no IT knowledge
D. Uses social media a lot
✅ **Answer: B**

**Q2.** What’s the safest way to open a resume from an unknown source?
A. Directly in Outlook
B. Download and unzip
C. Open in sandbox/preview mode
D. Forward to candidate
✅ **Answer: C**

**Q3.** Which of these is *not* considered PII?
A. Name
B. Company revenue
C. Aadhaar number
D. Email address
✅ **Answer: B**

**Q4.** What’s the correct way to share employee data with a background vendor?
A. Over WhatsApp
B. Encrypted file via official email
C. Personal Gmail
D. Shared Google Sheet
✅ **Answer: B**

**Q5.** “Right to be forgotten” means:
A. Employee can delete all emails
B. Candidate can request deletion of their data
C. HR must delete all records every month
D. None
✅ **Answer: B**

**Q6.** What’s the best way to protect HR systems?
A. Install random antivirus
B. Enable MFA & restrict access
C. Use free public Wi-Fi
D. Share passwords with team
✅ **Answer: B**

**Q7.** Which is a *safe* data disposal method?
A. Delete to recycle bin
B. Shred physical files / secure erase
C. Archive forever
D. Upload to Notion
✅ **Answer: B**

**Q8.** What should HR do after receiving a suspicious email with an attachment?
A. Delete it silently
B. Forward to IT/security team
C. Reply asking for details
D. Open and check content
✅ **Answer: B**

**Q9.** Which tool helps secure offer letters?
A. Paint
B. DocuSign
C. Notepad
D. Calculator
✅ **Answer: B**

**Q10.** What’s a good retention period for rejected candidates?
A. Forever
B. As per company policy (e.g., 6 months)
C. 10 years
D. None
✅ **Answer: B**

**Q11.** Which of these is a social engineering tactic?
A. Asking HR for salary info via fake call
B. Sending birthday cards
C. Posting ads
D. Scheduling meetings
✅ **Answer: A**

**Q12.** What’s the most common malware delivery format for HR attacks?
A. .zip or .docm attachments
B. .png image
C. .mp3 file
D. .txt file
✅ **Answer: A**

**Q13.** What is “least privilege”?
A. Everyone gets all access
B. Access only as per role
C. Only managers have passwords
D. Disable all access
✅ **Answer: B**

**Q14.** What’s the first action after discovering data leaked externally?
A. Delete all backups
B. Report immediately to IT/Security
C. Ignore if small
D. Inform the candidate directly
✅ **Answer: B**

**Q15.** Which regulation governs personal data protection in India?
A. PCI-DSS
B. DPDP Act 2023
C. GDPR
D. NIST
✅ **Answer: B**

✅ **Answer Key:** 1B, 2C, 3B, 4B, 5B, 6B, 7B, 8B, 9B, 10B, 11A, 12A, 13B, 14B, 15B

---

## 🎯 Outcomes

✅ HR staff understand **their role in safeguarding personal data.**
✅ Reduced phishing and fake job scam incidents.
✅ Enhanced trust among candidates and employees.
✅ Compliance with DPDP, GDPR, and internal data protection policies.
✅ HR becomes a **security partner**, not just an admin function.

> “Human Resources must protect the humans — and their data.” 💼

---

