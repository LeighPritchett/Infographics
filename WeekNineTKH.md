# Week 9 — Learning Summary

This week connected backend vulnerabilities, client‑side attack vectors, and API authorization flaws in a way that made the relationships between them much clearer. Each module built on the last, showing how SQLi, XSS/CSRF, and BOLA can appear in real applications and how attackers chain them together.

---

## Module 1 — SQL Injection (SQLi): Mechanics & Exploitation

### Summary
This module focused on understanding SQLi at a deeper, more technical level. I traced how user‑supplied input moves from the application interface into backend SQL queries, learned how to break query logic, and practiced using SQL operators to bypass authentication or extract data from unauthorized tables.

### Key Learning Objectives
- Map the lifecycle of user input as it flows into backend SQL query structures.
- Use the **single‑quote test** to identify vulnerable input fields and broken validation.
- Perform **authentication bypass** using tautologies like `OR 1=1` to force true evaluations.
- Execute **UNION‑based SQLi** to enumerate schemas and extract records from restricted tables.
- Reinforce why **parameterized queries** and strict **input sanitization** are essential defenses.

---

## Module 2 — XSS & CSRF: Client‑Side Attack Vectors

### Summary
This module explored how attackers target the browser instead of the server. I learned how reflected and stored XSS inject malicious scripts into the DOM, and how CSRF leverages authenticated sessions to force unintended actions on behalf of a user.

### Key Learning Objectives
- Differentiate **client‑side vs. server‑side** attack surfaces and understand how each impacts security.
- Execute **reflected XSS** by injecting malicious JavaScript into URL parameters.
- Deploy **stored XSS** to plant persistent payloads capable of stealing cookies or session data.
- Architect **CSRF attacks** that exploit automatic cookie‑sending to trigger unauthorized actions.

---

## Module 3 — API Security & BOLA: RESTful API Vulnerabilities

### Summary
This module focused on RESTful API traffic and how insecure object identifiers lead to Broken Object Level Authorization (BOLA). I practiced intercepting JSON requests, modifying object IDs, and identifying business logic flaws that attackers can exploit.

### Key Learning Objectives
- Intercept and analyze **RESTful API traffic** using Burp Suite as a MITM proxy.
- Exploit **BOLA/IDOR** by manipulating object IDs to access other users’ private data.
- Identify and abuse **business logic flaws**, such as bypassing discount or purchase restrictions.
- Explain how **rate limiting** and strict **input validation** protect APIs from brute‑force and abuse.

---

## Reflection
Week 9 helped me connect backend vulnerabilities, client‑side attacks, and API‑level authorization flaws in a practical way. Seeing SQLi, XSS/CSRF, and BOLA side‑by‑side made it easier to understand how attackers chain weaknesses across different layers of an application.
