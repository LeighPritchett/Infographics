**##Sources:##**

# **Week 4 — Virtualization → Containers → Orchestration**  
**Modules 1–3 Source Summary for NotebookLM**

---

## **Module 1 — Virtualization & Hypervisors**  
**(P1 • W4 • D1/T1 • M1 • S10)**

### **Learning Objectives**
- Differentiate Hypervisor Tiers: Type 1 (Bare Metal) vs. Type 2 (Hosted)  
- Engineer Virtual Perimeters: Configure Bridged, NAT, and Host‑Only networking  
- Architect a Sandbox: Build a forensic “Gold Standard” environment isolated from the local network

### **Core Ideas**
- Virtualization abstracts hardware; containers abstract the OS  
- Type 1 hypervisors run directly on hardware → stronger isolation, better performance  
- Type 2 hypervisors run on top of a host OS → more flexible but less isolated  
- Networking modes define exposure:  
  - **Bridged** = VM appears as a device on the LAN  
  - **NAT** = VM hides behind host’s IP  
  - **Host‑Only** = VM isolated from the internet  
- A proper sandbox requires strict boundaries so malware cannot escape

### **Takeaways**
- Virtualization is the foundation for safe experimentation  
- Networking choices directly affect security posture  
- A sandbox is more than “just a VM” — it’s an intentionally isolated environment

---

## **Module 2 — The Container Revolution**  
**(P1 • W4 • D2/T1 • M1 • S11)**

### **Learning Objectives**
- Differentiate Virtualization Models: VM hardware virtualization vs. Container OS virtualization  
- Master the Docker Trinity: Dockerfiles, Images, Containers  
- Execute Process Isolation: Use Linux namespaces for lightweight, isolated environments  
- Automate Deployment: Rapidly deploy and destroy a web server with no footprint

### **Core Ideas**
- Containers ≠ VMs — they’re isolated processes sharing the host kernel  
- Dockerfiles define environments; images package them; containers run them  
- Namespaces + cgroups = the isolation model that makes containers secure and lightweight  
- Automation makes environments reproducible and disposable

### **Takeaways**
- Containers solve “it works on my machine” by making environments portable  
- Understanding namespaces deepens the mental model of container isolation  
- Automation is key for repeatability, testing, and clean teardown  
- This module sets the stage for multi‑container systems and orchestration

---

## **Module 3 — Docker Compose & Orchestration**  
**(P1 • W4 • D3/T1 • M1 • S12)**

### **Learning Objectives**
- Translate Imperative to Declarative: Move from single Docker commands to YAML‑defined fleets  
- Orchestrate Microservices: Deploy dependent services (Web + Database) together  
- Engineer Virtual Switchboards: Create isolated FrontEnd and BackEnd bridge networks  
- Architect an Air‑Gap: Place a database in an internal‑only network

### **Core Ideas**
- Declarative YAML files describe the desired state of multi‑container systems  
- Docker Compose coordinates multiple services as one unit  
- Custom bridge networks control traffic flow and enforce boundaries  
- Air‑gapped databases reinforce the principle of least exposure

### **Takeaways**
- Compose makes multi‑service setups predictable and repeatable  
- Networking becomes intentional: public‑facing vs. internal‑only  
- Air‑gapping is a practical security pattern for sensitive data  
- This module is the conceptual bridge toward Kubernetes‑style orchestration

---

## **Week‑Level Synthesis**
Across these three modules, the progression is:

1. **Virtualization** — understanding hardware‑level isolation and network boundaries  
2. **Containers** — shifting to lightweight, process‑level isolation and automation  
3. **Orchestration** — managing multiple services declaratively with controlled networking

This week builds the mental model for modern infrastructure:  
from hypervisors → to containers → to multi‑service orchestration.

---

**Containers vs VMs: What's the difference?**
- https://www.youtube.com/watch?v=cjXI-yxqGTI

**Docker in 100 Seconds**
- https://www.youtube.com/watch?v=Gjnup-PuquQ

**Docker Compose will BLOW your MIND!! (a tutorial)**
- https://www.youtube.com/watch?v=DM65_JyGxCo

**The 3 Types of VirtualBox Networking**
- https://www.nakivo.com/blog/virtualbox-network-setting-guide/

**Docker Architecture**
- https://docs.docker.com/get-started/overview/

**Docker Networking Overview**
- https://docs.docker.com/network/