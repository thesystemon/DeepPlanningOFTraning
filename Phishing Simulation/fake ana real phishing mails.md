## 1 — Genuine: Vendor Invoice

**Subject:** Invoice INV-2025-451 — March supplies
**From:** SupplyCo Accounts [billing@supplyco.com](mailto:billing@supplyco.com)
**Body (snippet):** Please find attached invoice INV-2025-451 for ₹47,800. Payment due by 05-Apr-2025. Bank details on page 2.
**Action:** Pay to bank details in attached PDF after approval.
**Red flags (none):** Sender domain matches vendor, expected invoice, attachment is a signed PDF.

## 2 — Fake: Vendor Invoice (lookalike)

**Subject:** Invoice INV-2025-451 — March supplies
**From:** SupplyCo Accounts [billing@supp1yco.com](mailto:billing@supp1yco.com)
**Body (snippet):** Please find attached invoice INV-2025-451 for ₹47,800. Payment due by 05-Apr-2025. New bank details attached.
**Action:** Click the link to download invoice.
**Red flags:** Look-alike domain (supp1yco vs supplyco), asks to click link instead of opening known PDF, new bank details without prior notice.

---

## 3 — Genuine: HR Payslip Notification

**Subject:** Your March Payslip is Ready
**From:** HR Team [hr@yourcompany.com](mailto:hr@yourcompany.com)
**Body (snippet):** Hello Rahul, your March payslip is available in the HR portal. Login to view.
**Action:** Log in via internal HR portal (bookmark) to view payslip.
**Red flags (none):** Sent from corporate HR domain, expected monthly notice.

## 4 — Fake: HR Payslip Phish

**Subject:** Your March Payslip is Ready — Urgent
**From:** HR Team [payroll@yourcompany-hr.com](mailto:payroll@yourcompany-hr.com)
**Body (snippet):** Hello Rahul, your payslip is blocked. Click the link to re-verify your account or it will be locked.
**Action:** Click link and enter corporate credentials.
**Red flags:** Different domain (yourcompany-hr.com), urgent tone, asks for credentials via email link.

---

## 5 — Genuine: IT Password Reset (initiated by user)

**Subject:** Password reset confirmation
**From:** IT Helpdesk [it-help@yourcompany.com](mailto:it-help@yourcompany.com)
**Body (snippet):** You requested a password reset at 10:12 AM. If this was you, use the token sent to your phone. If not, contact IT.
**Action:** Use MFA token to confirm reset (no link in email).
**Red flags (none):** No link, expected flow, includes contact info for IT.

## 6 — Fake: IT Password Reset (credential harvest)

**Subject:** Immediate: Reset Your Password Now
**From:** IT Support [it-support@yourco-support.com](mailto:it-support@yourco-support.com)
**Body (snippet):** We detected suspicious activity. Click here to reset your password immediately to avoid lockout.
**Action:** Click link and enter username/password.
**Red flags:** Strange sending domain, link to external site, alarmist language.

---

## 7 — Genuine: Bank Alert (small business)

**Subject:** Alert: Scheduled Payment Processed
**From:** YourBank [noreply@yourbank.co.in](mailto:noreply@yourbank.co.in)
**Body (snippet):** A scheduled payment of ₹15,000 to Vendor X was processed on 28-Mar-2025. If this was not you, call us at 1800-XXX.
**Action:** Call bank using known number if suspicious.
**Red flags (none):** Known bank domain, instruction to call published phone.

## 8 — Fake: Bank Phish

**Subject:** Urgent: Payment Failed — Verify Account
**From:** YourBank [alerts@yourbank-secure.com](mailto:alerts@yourbank-secure.com)
**Body (snippet):** Payment to Vendor X failed. Verify your account now by clicking the secure link or your account will be suspended.
**Action:** Click link and provide account details.
**Red flags:** Strange domain, asks for sensitive banking info via link, threat of suspension.

---

## 9 — Genuine: LinkedIn Recruiter Message

**Subject:** Opportunity — Product Manager role
**From:** Priya Menon (Talent) [priya@recruitsolutions.com](mailto:priya@recruitsolutions.com) via LinkedIn
**Body (snippet):** Hi Neha — I saw your profile and would like to discuss a Product Manager role. Are you available for a quick call?
**Action:** Reply on LinkedIn or schedule via LinkedIn messaging.
**Red flags (none):** Contact arrived through LinkedIn, professional details visible.

## 10 — Fake: LinkedIn Phish (fake profile)

**Subject:** Exciting Opportunity — Interview today
**From:** Priya Menon [priya@recruits0lutions.com](mailto:priya@recruits0lutions.com)
**Body (snippet):** Hi Neha — We’ve shortlisted you. Please download the attached form and complete it to confirm your slot.
**Action:** Open attachment and fill in personal info.
**Red flags:** Email came from external address (not LinkedIn), look-alike domain, asks for sensitive personal info via attachment.

---

## 11 — Genuine: Cloud Document Share

**Subject:** [Google Drive] Access granted: Q2 Budget.xlsx
**From:** Finance Team [no-reply@docs.google.com](mailto:no-reply@docs.google.com)
**Body (snippet):** You have been granted view access to Q2 Budget.xlsx by [finance@yourcompany.com](mailto:finance@yourcompany.com) via Google Drive. Open in Drive to view.
**Action:** Open document from Google Drive UI (check owner).
**Red flags (none):** Link points to drive.google.com, owner is verified.

## 12 — Fake: Cloud Share Phish

**Subject:** [Google Drive] Shared Document: Q2 Budget.xlsx
**From:** Google Docs [no-reply@googledocs-share.com](mailto:no-reply@googledocs-share.com)
**Body (snippet):** [finance@yourcompany.com](mailto:finance@yourcompany.com) shared Q2 Budget. Click here to view — login required.
**Action:** Click and log in on presented page (credential harvest).
**Red flags:** Non-Google domain, asks for login on external page, urgency to “allow access.”

---

## 13 — Genuine: Vendor Bank Change Request (internal process)

**Subject:** Vendor Bank Update Request — Vendor X
**From:** VendorX Finance [accounts@vendorx.com](mailto:accounts@vendorx.com)
**Body (snippet):** Hello Accounts — Please find attached a signed form for bank account update for Vendor X. Please process only after our official verification call.
**Action:** Follow dual-approval and verify by phone before changing details.
**Red flags (none):** Mentions verification step and is from known vendor domain.

## 14 — Fake: Vendor Bank Change Phish

**Subject:** URGENT: Vendor Bank Details Updated — Vendor X
**From:** VendorX Finance [accounts@vendorx-payments.com](mailto:accounts@vendorx-payments.com)
**Body (snippet):** Please update your records — the vendor’s bank has changed. Click the attached file to update the vendor in your system. Payment pending.
**Action:** Open attachment and update payee details.
**Red flags:** New/unknown vendor domain, immediate payment pressure, no verification instruction.

---

## 15 — Genuine: CEO Request (internal, via known channel)

**Subject:** Quick approval needed — Invoice #998
**From:** CEO Office [ceo@yourcompany.com](mailto:ceo@yourcompany.com) via internal mail
**Body (snippet):** Hi Team — Please route invoice #998 to Finance for approval. I’ll join the call in 10 min.
**Action:** Forward to Finance as usual; confirm via Teams if unsure.
**Red flags (none):** Sent through internal verified mailbox, known cadence.

## 16 — Fake: CEO Fraud (CEO impersonation)

**Subject:** URGENT — Wire transfer now (confidential)
**From:** John Sharma [john@yourcompany-corp.com](mailto:john@yourcompany-corp.com)
**Body (snippet):** Hi — I need a wire transfer of ₹8,00,000 to the account in the attached form. Do it now and mark confidential. — John
**Action:** Send funds immediately.
**Red flags:** Slightly different domain, urgent confidential tone, bypasses normal approval process.

---

## 17 — Genuine: Calendar Invite (internal)

**Subject:** Q1 Review — 10 Apr 11:00 AM (Teams meeting)
**From:** Calendar [calendar@yourcompany.com](mailto:calendar@yourcompany.com)
**Body (snippet):** You are invited to join the Q1 review. Join via Teams link in the invite.
**Action:** Accept via corporate calendar.
**Red flags (none):** Calendar invite from internal system, Teams link uses company tenant.

## 18 — Fake: Malicious Calendar Invite

**Subject:** Urgent Meeting — Join now
**From:** Meeting Room [notifications@calendar-service.com](mailto:notifications@calendar-service.com)
**Body (snippet):** Click link to join meeting: [https://join-now.example/meeting123](https://join-now.example/meeting123) — requires sign-in to proceed.
**Action:** Click external link and sign in.
**Red flags:** External calendar domain, link goes to non-Teams URL, asks to sign in via page that is not corporate SSO.

---

## 19 — Genuine: Delivery Notification (known courier)

**Subject:** Delivery Scheduled: Parcel #7643 — Action Required
**From:** FastShip [noreply@fastship.in](mailto:noreply@fastship.in)
**Body (snippet):** Your parcel is scheduled for delivery on 02-Apr. If you’re unavailable, reschedule using our portal. Tracking: [track.fastship.in/7643].
**Action:** Track using courier’s official tracking page.
**Red flags (none):** Domain matches courier, tracking link points to official domain.

## 20 — Fake: Smishing/Delivery Phish (email variant)

**Subject:** Missed Delivery — Claim Parcel Now
**From:** FastShip [support@fastsh1p.com](mailto:support@fastsh1p.com)
**Body (snippet):** We attempted delivery. Click here to confirm address and pay ₹49 shipping to release parcel.
**Action:** Click link and enter card details.
**Red flags:** Look-alike domain (fastsh1p), asks for payment on small fee, not expected.

---

### How to use these in training

* **Spot-the-phish**: Show pairs (genuine vs fake) and ask trainees to identify the 2–3 red flags in the fake one.
* **Discussion prompts**: “If you received the fake Vendor Bank Change email, what are the three immediate steps?” (Verify by phone, do not click, report).
* **Simulated phish**: Use these templates (redacted) in a controlled phishing simulation to measure click rates.

---

