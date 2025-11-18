# Deployment and Testing of Open-source IP-PBX Solution (FreePBX)

This repository contains the screenshots, documentation, and presentation for the project **“Deployment and Testing of Open-source IP-PBX Solution for Real-time Communication”**, implemented using **FreePBX on CentOS (VMware)**.



# Project Overview
This project demonstrates the complete deployment and testing of an open-source IP-PBX system using **FreePBX**, covering:

- Installation of CentOS on VMware  
- Static IP configuration  
- Installation of FreePBX and required modules  
- Creation and configuration of SIP extensions  
- Registration of softphones (Zoiper, 3CX)  
- Test call setup between extensions  
- Packet capturing using Wireshark  
- SIP & RTP flow analysis  
- Verification of call signaling and media transfer  

This project shows how organizations can use FreePBX for secure, reliable, and cost-effective VoIP communication.

# Tools & Technologies Used

## **Software & Platforms**
- VMware Workstation  
- CentOS (Linux environment)  
- FreePBX (Open-source IP-PBX)  
- Asterisk  
- PuTTY (SSH remote access)  
- WinSCP (Secure file transfer)  
- Zoiper & 3CX (Softphone clients)  
- Wireshark (Packet Analysis)

## **Protocols & Concepts**
- SIP (Session Initiation Protocol)  
- RTP (Real-time Transport Protocol)  
- VoIP (Voice over IP)  
- Codecs (G.711, G.729, etc.)  
- Static IP configuration  
- Linux commands & services  
- Firewall rules  
- SIP call flows & message headers  

---

## Implementation Workflow
1. **Create a CentOS VM** using VMware  
2. **Configure a static IP** inside CentOS  
3. **Install dependencies** (Apache, MySQL/MariaDB, PHP, Asterisk)  
4. **Install FreePBX** and start services  
5. **Access the FreePBX web GUI** using browser  
6. **Create SIP extensions** (e.g., 3001, 3002)  
7. **Configure softphones** (Zoiper / 3CX) with extension credentials  
8. **Perform internal extension-to-extension calls**  
9. **Capture SIP & RTP packets** using Wireshark  
10. **Analyze the call flow** (INVITE, RINGING, OK, ACK, BYE)  
11. **Validate RTP audio stream** using packet capture  
12. **Verify successful call setup, media flow, and teardown**

---

# SIP Call Flow Tested
- INVITE  
- 100 TRYING  
- 180 RINGING  
- 200 OK  
- ACK  
- RTP Media Stream  
- BYE  
- 200 OK (Call terminated)

Wireshark screenshots for call signaling and RTP flow are included in the `/screenshots` folder.

---

# Results & Observations
- FreePBX installed successfully on CentOS VM  
- Softphones registered and authenticated without issues  
- Internal calls between extensions worked perfectly  
- SIP packet flow matched expected behavior  
- RTP media packets verified in Wireshark  
- Firewall and security configurations applied  
- System achieved stable, high-quality audio communication  

---

# Security Measures Implemented
- Strong SIP passwords for all extensions  
- FreePBX firewall enabled  
- Fail2Ban activated  
- Access restricted to LAN only  
- SSH secured via PuTTY  
- Sensitive data removed before uploading to GitHub  

---

# References
- FreePBX Official Documentation  
- Asterisk VoIP Architecture Papers  
- SIP RFC 3261  
- Linux Administration Guides  
- Research papers referenced in project PPT  

---

# Author
**Keerthana S (E0322005)**  
B.Tech AI & Data Analytics  
Project: *Deployment and Testing of Open-source IP-PBX Solution*  

---

