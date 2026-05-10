# Week 8 — Learning Summary

This week focused on strengthening my understanding of web application vulnerabilities across SQL Injection, XSS/CSRF, and API‑level flaws. Each module built on the last, helping me connect how different attack surfaces interact in real applications.

---

## Module 1 — SQL Injection (SQLi)

### Summary
This module explored how SQL Injection works at a deeper level by tracing how user input flows into backend SQL queries. I practiced identifying weak validation points, breaking query logic, and using SQL operators to bypass authentication or extract data.

### Key Learning Objectives
- Map how user‑supplied input is integrated into backend SQL queries.
- Use the **single‑quote test** to detect broken input validation.
- Perform **authentication bypass** using tautologies like `' OR 1=1 --`.
- Execute **UNION‑based SQLi** to enumerate schemas and extract sensitive data.
- Understand why **parameterized queries** and **input sanitization** are the only reliable defenses.

---

## Module 2 — XSS & CSRF

### Summary
This module shifted the focus to client‑side vulnerabilities. I learned how malicious scripts can be injected into the browser through reflected or stored XSS, and how CSRF abuses authenticated sessions to force unintended actions.

### Key Learning Objectives
- Differentiate **client‑side vs. server‑side** attack surfaces.
- Execute **reflected XSS** via malicious URL parameters.
- Deploy **stored XSS** to plant persistent scripts for cookie/session theft.
- Understand how **CSRF** leverages automatic cookie‑sending to perform unauthorized actions.

---

## Module 3 — API Security & BOLA

### Summary
This module focused on RESTful API vulnerabilities, especially how insecure object identifiers lead to Broken Object Level Authorization (BOLA). I practiced intercepting JSON traffic, modifying IDs, and identifying business logic flaws.

### Key Learning Objectives
- Intercept and analyze **RESTful API traffic** using Burp Suite.
- Exploit **BOLA/IDOR** by manipulating object IDs to access unauthorized data.
- Identify and abuse **business logic flaws**, such as bypassing discount restrictions.
- Explain why **rate limiting** and strict input validation protect APIs from brute‑force and abuse.

---

## Reflection
Week 8 helped me understand how backend, client‑side, and API vulnerabilities all fit together. Seeing SQLi, XSS/CSRF, and BOLA in sequence made the relationships between these attack surfaces much clearer and gave me a stronger foundation for the hands‑on labs that followed.
