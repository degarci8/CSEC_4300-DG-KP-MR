# CSEC 4300 Malware Analysis Project  
### ShadowV2 IoT Botnet Analysis

---

## 👥 Team Members
- Kyle  
- Derek Garcia  
- Michael  

---

## 🦠 Malware Focus  
**ShadowV2** – A Mirai-based IoT botnet targeting vulnerable embedded and Linux-based devices.

---

## 📌 Project Overview  
This project focuses on the reverse engineering and behavioral analysis of ShadowV2 malware. The goal is to simulate a real-world malware analysis workflow by combining static, dynamic, and memory analysis techniques within a controlled lab environment.

Through this project, we aim to:
- Understand how IoT malware infects and propagates  
- Analyze command-and-control (C2) communication patterns  
- Identify indicators of compromise (IOCs)  
- Develop detection and mitigation strategies  

---

## 🧠 Key Learning Objectives
- Perform **static and dynamic malware analysis**
- Analyze **assembly-level instructions and obfuscation techniques**
- Investigate **runtime behavior and system impact**
- Build a **secure, isolated malware analysis lab**
- Apply **defensive strategies used in SOC environments**

---

## 🏗️ Lab Environment Architecture  

This project is conducted in a **segmented and isolated virtual lab** to safely analyze malware behavior.

### 🔐 Key Features:
- VLAN segmentation to isolate infected systems  
- No outbound internet access for malware VLAN  
- Controlled traffic monitoring and logging  
- VPN access for team collaboration  
- Virtualized infrastructure using hypervisors  

### ⚙️ Technologies Used:
- Virtual Machines (Linux-based analysis systems)  
- Network segmentation (VLANs)  
- Packet analysis tools (e.g., Wireshark)  
- Debugging tools (e.g., x64dbg / GDB)  
- System monitoring tools (e.g., Procmon, Process Explorer)  

---

## 🔬 Project Phases  

### 1. Environment Setup  
- Build isolated malware analysis lab  
- Configure VLANs and firewall rules  
- Deploy analysis VMs  

### 2. Static Analysis  
- Examine binaries without execution  
- Extract strings, imports, and metadata  
- Identify obfuscation techniques  

### 3. Assembly-Level Analysis  
- Reverse engineer using disassemblers/debuggers  
- Trace execution flow  
- Analyze key functions and payload logic  

### 4. Dynamic & Memory Analysis  
- Execute malware in sandboxed environment  
- Monitor system changes and network activity  
- Capture memory artifacts  

### 5. Behavior & Defense  
- Identify attack patterns and persistence mechanisms  
- Extract IOCs (IPs, domains, file hashes)  
- Recommend detection and mitigation strategies  

---

## 📊 Key Findings (Work in Progress)
- ShadowV2 targets **IoT and Linux-based systems**
- Uses **botnet architecture for distributed attacks (DDoS)**
- Leverages **hardcoded credentials and scanning techniques**
- Establishes communication with **C2 infrastructure**

---

## 🛡️ Detection & Mitigation Strategies  
- Network segmentation and strict firewall rules  
- Disable unused services on IoT devices  
- Enforce strong authentication (no default credentials)  
- Monitor for unusual outbound traffic  
- Deploy IDS/IPS solutions for anomaly detection  

---

## 📚 Documentation  
Detailed analysis, notes, and findings are maintained in the **GitHub Wiki**:  
👉 https://github.com/degarci8/CSEC_4300-DG-KP-MR/wiki  

---

## ⚠️ Security Disclaimer  
Malware binaries are **NOT stored in this repository** to prevent accidental misuse or distribution.

This project is strictly for **educational and research purposes** within a controlled environment.

---

## 🚀 Future Improvements  
- Integrate ELK/SIEM for log analysis  
- Automate IOC extraction  
- Expand analysis to additional IoT malware families  
- Develop detection rules (Sigma / Snort / Suricata)  

---

## 📎 Skills Demonstrated  
- Malware Analysis & Reverse Engineering  
- Network Security & Traffic Analysis  
- Virtual Lab Design & Isolation  
- Threat Detection & Incident Response  
- Linux & System-Level Debugging  
