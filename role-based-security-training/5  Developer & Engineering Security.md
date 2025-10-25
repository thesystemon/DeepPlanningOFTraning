# 📘 Chapter 5 — Developer & Engineering Security

*(Secure Coding | Secret Management | Vulnerability Prevention)*

---

## 🧠 Learning Objectives

By the end of this chapter, developers and engineers will be able to:
✅ Understand the importance of secure coding and its impact on overall security.
✅ Identify and avoid common coding vulnerabilities (OWASP Top 10).
✅ Properly handle credentials, API keys, and environment secrets.
✅ Implement DevSecOps and CI/CD pipeline security controls.
✅ Use automated tools to detect insecure dependencies and code issues.
✅ Integrate security in every stage of software development — “Shift Left Security”.

---

## 📚 Slide / PDF Content — In Depth

---

### **Slide 1 — “Code is Power — and Responsibility”**

> “Every line of code can either protect or expose your organization.”

Developers and engineers have unique power — their work defines how securely data is stored, transmitted, and processed. A small mistake like leaving a key in GitHub can expose entire systems.

💡 **Key Threats Developers Face:**

* Exposed secrets (API keys, DB passwords)
* Injection vulnerabilities (SQL, XSS, Command Injection)
* Insecure deserialization
* Outdated dependencies (vulnerable libraries)
* Weak authentication logic
* Misconfigured CI/CD pipelines

🧩 **Example:**
In 2022, a fintech startup exposed AWS keys in GitHub — resulting in complete S3 data leakage within 24 hours.

---

### **Slide 2 — Secure Coding Mindset (Shift Left Security)**

Traditional security → Tested *after* code is written.
Modern security → Built *into* every development step.

| Stage           | Secure Practice                        |
| --------------- | -------------------------------------- |
| **Design**      | Threat modeling, data classification   |
| **Development** | Input validation, least privilege code |
| **Testing**     | SAST/DAST scanning, secure unit tests  |
| **Deployment**  | Hardening, secret management           |
| **Maintenance** | Patch dependencies, monitor for CVEs   |

🧩 Tip: Treat security bugs like functional bugs — **track and fix** them with equal priority.

---

### **Slide 3 — Common Vulnerabilities (OWASP Top 10)**

| Vulnerability                   | Example                       | Prevention                     |
| ------------------------------- | ----------------------------- | ------------------------------ |
| **Injection**                   | SQL: `' OR 1=1--`             | Use prepared statements        |
| **Broken Auth**                 | Weak login logic              | Implement JWT + bcrypt         |
| **Sensitive Data Exposure**     | Unencrypted DB                | Encrypt at rest and in transit |
| **XXE**                         | XML parser attack             | Disable external entities      |
| **Insecure Deserialization**    | Object injection              | Validate serialized input      |
| **Security Misconfiguration**   | Default creds, open S3 bucket | Harden configurations          |
| **XSS**                         | `<script>alert(1)</script>`   | Sanitize user inputs           |
| **CSRF**                        | Forged web requests           | Use CSRF tokens                |
| **Using Vulnerable Components** | Outdated libraries            | Use dependency scanning        |
| **Insufficient Logging**        | No monitoring                 | Enable audit logging           |

🧩 Activity: Show code examples of SQL Injection and secure prepared statement equivalent.

---

### **Slide 4 — Secret Management (API Keys, Passwords, Tokens)**

> “Hardcoded credentials = open door for attackers.”

| Don’t                          | Do                                                       |
| ------------------------------ | -------------------------------------------------------- |
| Store API keys in code         | Use secret vaults (HashiCorp Vault, AWS Secrets Manager) |
| Commit `.env` files to Git     | Add `.env` to `.gitignore`                               |
| Share secrets in Slack/email   | Use password vault or secure channels                    |
| Use same key for all services  | Rotate keys regularly                                    |
| Store private keys unencrypted | Use key management system (KMS)                          |

🧩 Example:
`config.js` → contains `db_password = "admin123"` → if pushed to GitHub, it’s automatically scanned by bots within minutes.

---

### **Slide 5 — Dependency & Package Security**

> “You inherit every vulnerability your library has.”

| Area                                  | Best Practice                                          |
| ------------------------------------- | ------------------------------------------------------ |
| **Dependencies**                      | Use trusted repos only (npm, Maven Central)            |
| **Versioning**                        | Pin exact versions in `package-lock.json` or `pom.xml` |
| **Scanning**                          | Run `npm audit`, `mvn dependency:check`, or `Snyk`     |
| **Update Policy**                     | Regularly patch and test                               |
| **SBOM (Software Bill of Materials)** | Maintain list of components used for compliance        |

🧩 Tip: Never use “latest” tag in Dockerfiles — it can silently pull insecure images.

---

### **Slide 6 — Secure DevOps & CI/CD Practices**

| Area                       | Secure Practice                                      |
| -------------------------- | ---------------------------------------------------- |
| **Pipeline Security**      | Run builds in isolated runners                       |
| **Code Signing**           | Sign artifacts before release                        |
| **Static Analysis (SAST)** | Integrate SonarQube / CodeQL into pipeline           |
| **Dependency Scanning**    | Automate with Snyk, Dependabot                       |
| **Container Security**     | Use Trivy or Clair for image scanning                |
| **Secrets in Pipelines**   | Use vaults, not environment variables in YAML        |
| **Access Control**         | Use least privilege for build agents                 |
| **Logging & Alerts**       | Monitor failed build patterns or suspicious activity |

🧩 Example:
Add a “Security Stage” in Jenkins → fails build if vulnerability severity ≥ High.

---

### **Slide 7 — Vulnerability Prevention Checklist (Developer Level)**

| Area             | Checklist Item                      | Status |
| ---------------- | ----------------------------------- | ------ |
| Input Validation | All inputs validated & sanitized    | ☐      |
| Authentication   | Strong password & MFA logic         | ☐      |
| Authorization    | Role-based access enforced          | ☐      |
| Error Handling   | No sensitive info in errors         | ☐      |
| Secrets          | Stored in vault, not code           | ☐      |
| Logging          | Secure, centralized, non-repudiable | ☐      |
| Dependencies     | Regularly scanned & updated         | ☐      |
| HTTPS            | Enforced sitewide                   | ☐      |
| API Security     | Tokens validated, rate-limited      | ☐      |
| Code Review      | Peer-reviewed for security          | ☐      |

🧩 Add this checklist to every **pull request** or **pre-release QA review**.

---

### **Slide 8 — Code Review & Peer Validation**

> “Two eyes see bugs, four eyes prevent breaches.”

* Use **code review templates** with security checkpoints.
* Focus on:

  * Input/output handling
  * Authentication logic
  * Access control boundaries
  * Data encryption
  * Logging and exception handling

🧩 Tip: Automate code review for secrets using **GitGuardian / TruffleHog**.

---

### **Slide 9 — Secure Build and Deployment**

| Phase                      | Key Action                                |
| -------------------------- | ----------------------------------------- |
| **Build**                  | Sign packages, hash verify outputs        |
| **Deploy**                 | Use secured pipelines and MFA             |
| **Environment Config**     | Use `.env` files managed by vault         |
| **Rollback Plan**          | Always maintain a secure version rollback |
| **Post-Deploy Monitoring** | Monitor for anomalies and abuse patterns  |

🧩 Example:
Add automated test → verifies all HTTPS requests, rejects HTTP by default.

---

### **Slide 10 — Developer Security Checklist**

# | Task | Status

--|------|--------
1 | Enable SAST/DAST scanning in CI/CD | ☐
2 | Use secret vault for all keys and tokens | ☐
3 | Enforce code review for security issues | ☐
4 | Scan all containers and dependencies | ☐
5 | Avoid hardcoding credentials or URLs | ☐
6 | Use HTTPS/TLS for all endpoints | ☐
7 | Apply input validation and encoding | ☐
8 | Perform threat modeling per module | ☐
9 | Implement security logging | ☐
10 | Patch third-party libraries monthly | ☐

---

### **Slide 11 — Key Takeaways**

✅ Security starts at the **first line of code**, not production.
✅ Follow **least privilege**, **secret vaulting**, and **dependency scanning**.
✅ Automate everything possible — security should not slow down development.
✅ Review, audit, and document all security configurations.
✅ Dev + Sec + Ops = DevSecOps — *a culture, not a tool.*

> “Great code runs fast. Secure code runs forever.” ⚡

---

## 🧩 Interactive Activities

| Activity                   | Description                                                  |
| -------------------------- | ------------------------------------------------------------ |
| **Secret Hunt Drill**      | Scan Git repo with GitGuardian / TruffleHog to find secrets. |
| **Code Fix Workshop**      | Fix an SQL injection vulnerability in a sample codebase.     |
| **Dependency Audit**       | Run `npm audit` or `mvn dependency:check` on live project.   |
| **Pipeline Security Demo** | Add security scanning stage in Jenkins or GitHub Actions.    |

---

## 🧰 Recommended Tools for Developers & Engineers

| Tool                            | Purpose                             | Type              |
| ------------------------------- | ----------------------------------- | ----------------- |
| **SonarQube / CodeQL**          | Static code analysis                | SAST              |
| **OWASP ZAP / Burp Suite**      | Dynamic app testing                 | DAST              |
| **Trivy / Clair**               | Container image scanning            | DevSecOps         |
| **GitGuardian / TruffleHog**    | Secret detection                    | Git Security      |
| **Snyk / Dependabot**           | Dependency vulnerability management | Package Security  |
| **Vault / AWS Secrets Manager** | Secret storage                      | Secret Management |
| **Threat Dragon**               | Visual threat modeling              | Design Security   |

---

## 🧮 15 MCQs — Developer & Engineering Security

**Q1.** What is “secure coding”?
A. Code that is optimized for performance
B. Code written with security best practices
C. Code that only runs on Linux
D. Code without comments
✅ **Answer: B**

**Q2.** What should you do with secrets in your code?
A. Store in GitHub
B. Store in secret vault
C. Email them to teammates
D. Encrypt manually and commit
✅ **Answer: B**

**Q3.** Which of these prevents SQL Injection?
A. String concatenation
B. Prepared statements
C. Inline queries
D. HTML encoding
✅ **Answer: B**

**Q4.** Which tool scans for secrets in code?
A. GitGuardian
B. Notepad
C. Excel
D. Jenkins
✅ **Answer: A**

**Q5.** What does OWASP stand for?
A. Online Web Application Security Project
B. Open Web Application Security Project
C. Open Web App Secure Program
D. Organization for Web Application Safety Protocol
✅ **Answer: B**

**Q6.** What’s the main goal of DevSecOps?
A. Add security throughout development lifecycle
B. Delay security till production
C. Replace developers with tools
D. Eliminate DevOps
✅ **Answer: A**

**Q7.** What is dependency scanning used for?
A. Checking outdated or vulnerable libraries
B. Counting lines of code
C. Optimizing performance
D. Tracking user sessions
✅ **Answer: A**

**Q8.** Which file should not be committed to Git?
A. `.env`
B. `README.md`
C. `package.json`
D. `index.html`
✅ **Answer: A**

**Q9.** Why should you use HTTPS?
A. Encrypt data in transit
B. Reduce bandwidth
C. Improve page speed
D. Disable JavaScript
✅ **Answer: A**

**Q10.** What is the best way to handle 3rd-party libraries?
A. Pin versions and scan for vulnerabilities
B. Download from random sources
C. Ignore updates
D. Modify without review
✅ **Answer: A**

**Q11.** Which is part of OWASP Top 10?
A. XSS
B. Network lag
C. DNS cache
D. UI bug
✅ **Answer: A**

**Q12.** What is “Shift Left Security”?
A. Fixing security issues earlier in development
B. Moving servers to left rack
C. Outsourcing security
D. Ignoring security in early stages
✅ **Answer: A**

**Q13.** What prevents hardcoded secrets?
A. Vault or KMS
B. Code comments
C. Logging system
D. Static import
✅ **Answer: A**

**Q14.** Which practice helps maintain accountability?
A. Code review & audit logging
B. Using shared accounts
C. Deleting logs
D. Avoiding pull requests
✅ **Answer: A**

**Q15.** What is the best security control for APIs?
A. Token-based authentication and rate limiting
B. Open access without validation
C. Use of GET for sensitive data
D. Logging off all requests
✅ **Answer: A**

✅ **Answer Key:** 1B, 2B, 3B, 4A, 5B, 6A, 7A, 8A, 9A, 10A, 11A, 12A, 13A, 14A, 15A

---

## 🎯 Outcomes

✅ Developers adopt “secure-by-design” and “shift-left” mindset.
✅ Secrets and credentials handled securely.
✅ Automated vulnerability scanning integrated into pipelines.
✅ Reduced risk from insecure code and outdated dependencies.
✅ Engineering becomes a **proactive security force**, not a reactive one.

> “Security isn’t a blocker for innovation — it’s what keeps innovation alive.” 💻🔒

---

