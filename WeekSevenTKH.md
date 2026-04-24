# **Week 7 — Reconnaissance, Scanning & Vulnerability Analysis**  
_This Week I Learned — The Perimeter (Sprint 2, Week 7)_

---

## **Source 1 — Week 7 Overview (The Perimeter)**  
**Focus:** Reconnaissance, Scanning & Vulnerability Analysis  

For six weeks, the emphasis was on building and hardening systems. Week 7 marks the shift into Sprint 2, where the role changes from engineer to scout. This week introduces Phase 1 of the Cyber Attack Lifecycle: **Reconnaissance**.  
Key ideas include passive intelligence gathering, mapping digital footprints, scanning networks for open services, and triaging vulnerability reports using real‑world risk instead of score alone.  
The mindset: **offense‑informed defense**.

---

## **Source 2 — Cyber Intelligence / OSINT Learning Objectives**  
**Key Concepts & Skills:**  
- **Execute the Intelligence Cycle:** Direct → Collect → Analyze public data to map a target’s tech stack without touching their servers.  
- **Google Dorking:** Identify leaked environment variables, exposed directories, and indexed backup files.  
- **Shodan Mastery:** Filter by geography, vulnerability status, and service type to identify exposed public‑facing systems.  
- **Threat Profile Reporting:** Combine subdomain enumeration, credential leak checks, and tech stack analysis to build a complete threat profile.

---

## **Source 3 — Network Scanning & Enumeration Learning Objectives**  
**Key Concepts & Skills:**  
- **TCP Handshake Breakdown:** SYN → SYN‑ACK → ACK and what each state reveals about a port or service.  
- **Host Discovery:** Use ICMP ping sweeps to identify live hosts without triggering alarms.  
- **Service Enumeration:** Use Nmap flags (`-sV`, `-p-`) to identify open ports, running services, and software versions.  
- **Output Translation:** Convert raw terminal scan results into a clean, professional network enumeration map.

---

## **Source 4 — Vulnerability Analysis Learning Objectives**  
**Key Concepts & Skills:**  
- **CVE & CVSS Interpretation:** Understand vulnerability scoring and why a CVSS 10.0 is not always the top priority.  
- **Automated Audits:** Use Nikto to identify outdated software and known‑bad configurations.  
- **False Positive Identification:** Distinguish theoretical vulnerabilities from actual, exploitable threats.  
- **Risk Triage:** Apply the formula **Risk = Likelihood × Impact** to justify remediation priorities.

---

## **Source 5 — End‑of‑Week 7 Outcomes**  
By the end of Week 7, Fellows will be able to:  
- Execute passive reconnaissance using OSINT tools and public search engines without triggering alerts.  
- Deploy Nmap for host discovery, port scanning, and service version enumeration.  
- Interpret CVE/CVSS data with real‑world context.  
- Triage a live vulnerability report using the Likelihood × Impact framework.  
- Produce a structured, defensible remediation plan.

---

## **Summary**  
Week 7 marks the transition from internal system building to external perimeter analysis. The focus is on understanding how attackers gather information, how networks reveal themselves through scanning, and how vulnerabilities must be triaged based on real‑world risk. This week builds the foundation for thinking like a defender who understands the offensive perspective.

