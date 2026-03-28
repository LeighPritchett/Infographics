# Week 3 — Master Sources

## **This Week I Learned — Python as a Security Tool**

This week, we shifted from using Python as a general scripting language to using it as a **security tool inside a headless VM**. Working without a GUI forced me to think like a defender: how do you automate checks, analyze logs, and understand system behavior when all you have is the terminal?

Across several labs, I built scripts that could analyze logs, detect suspicious processes, check for vulnerable ports, and generate structured reports. These exercises showed how Python can support real security workflows through automation and logic.

---

# 🔧 **Technical Learning**

## **1. Translating Security Policy to Logic**
- Converted verbal access rules into Python `if/else` structures  
- Used logic to allow or deny traffic based on IPs, ports, or patterns  
- Practiced clean indentation (“Law of White Space”) to structure decisions  

## **2. Data Types as Security Evidence**
- **Strings** → IP addresses  
- **Integers** → port numbers  
- **Lists** → scan targets or host groups  
- Treated data types as structured evidence for automated analysis  

## **3. Network Sensing & Automation**
- Built “efficiency engines” using `for` loops to automate repetitive checks  
- Used the `socket` library to test whether ports were open or closed  
- Detected unauthorized services or exposed ports on the VM  

## **4. Safe File Handling & Persistence**
- Used `with open()` to prevent file corruption and memory leaks  
- Practiced reading (`r`), writing (`w`), and appending (`a`) security data  
- Stored findings and logs safely for later review  

## **5. Defensive Coding**
- Implemented `try/except` blocks to handle missing logs or permission errors  
- Ensured scripts stayed stable under unexpected system conditions  

## **6. Forensic Filtering & Reporting**
- Parsed raw system logs to extract meaningful events  
- Simulated early‑stage incident response through log analysis  
- Generated structured reports like `brute_report.txt`  

## **7. OS Integration & System Automation**
- Used `subprocess` to run native Bash commands from Python  
- Captured command output with `capture_output=True` for deeper analysis  
- Verified environment paths and file existence using the `os` library  

## **8. JSON Alerts & System Auditing**
- Created machine‑readable alerts using the `json` library  
- Matched the format used by SIEM and SOC tools  
- Built a functional `system_auditor.py` script to detect unauthorized processes  

---

# 🧭 **Career Development — SMART Goals**

## **SMART Framework**
- Set goals that are Specific, Measurable, Achievable, Relevant, and Time‑bound  
- Focused on clarity and realistic expectations  

## **Short‑Term Goals for Motivation**
- Broke large objectives into smaller steps  
- Used short‑term wins to build momentum and avoid burnout  

## **Long‑Term Alignment**
- Connected daily tasks to long‑term career direction  
- Used deadlines and structure to stay accountable  

---

# 📁 **Files Created This Week**
- `incident_response.py` — 36 lines added  
- `threat_report.json` — 8 lines added  

---

# **Summary**
This week reinforced how Python can function as a practical security instrument. By combining logic, automation, file handling, and OS integration, I built tools capable of detecting anomalies, analyzing logs, checking ports, and generating structured reports. It’s becoming clearer how these foundational skills support real‑world security operations.