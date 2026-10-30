<div align="center">

# 🦈 Wireshark Practical Labs & Packet Analysis

**Building practical network traffic inspection and security troubleshooting capabilities using Wireshark**
</div>

<p align="center">
<img src="https://img.shields.io/badge/Skill-Packet%20Analysis-404040?style=flat-square&labelColor=C00000" />
<img src="https://img.shields.io/badge/Tool-Wireshark%20v4.x-1679AB?style=flat-square&labelColor=000000&logo=wireshark&logoColor=white" />
<img src="https://img.shields.io/badge/Protocol-TCP%2FIP-E87500?style=flat-square&labelColor=000000" />
<img src="https://img.shields.io/badge/Skill-Network%20Security-404040?style=flat-square&labelColor=C00000" />
<img src="https://img.shields.io/badge/Filtering-Display%20Filters-238F89?style=flat-square&labelColor=000000" />
<img src="https://img.shields.io/badge/SOC%20Analysis-C00000?style=flat-square&labelColor=000000" />
<img src="https://img.shields.io/badge/GitHub-404040?style=flat-square&labelColor=0070C0&logo=github&logoColor=white" />
<img src="https://img.shields.io/badge/NetworkWalks-404040?style=flat-square&labelColor=000000" />
<img src="https://img.shields.io/badge/Malek%20Aroua-CC0000?style=flat-square" />
</p>

---

## 📌 Project Overview

This project documents hands-on practical exercises, packet capture investigations, and network troubleshooting scenarios using **Wireshark**. 

The repository is structured to break down fundamental packet filtering, TCP/IP handshakes, and security investigation techniques into clean, documented lab modules.

---

## 🎯 Objectives

The main goals of these practical labs are:
- Master the Wireshark interface, packet list panes, and raw byte inspection.
- Apply essential display filters to isolate specific hosts, protocols, and ports.
- Analyze connection establishment (`SYN`, `SYN-ACK`, `ACK`), data transmission, and termination mechanics (`FIN`, `RST`).
- Investigate network reconnaissance, service availability, and potential security anomalies.

---

## 🛡️ Scope of the Labs

This repository covers core networking and analysis scenarios:
- **Lab 1:** Introduction to Wireshark & Basic Display Filtering (`ip.addr`, `tcp.port`, `dns`, `http`).
- **Lab 2:** TCP Handshake & Traffic Flow Analysis (Tracking flags, sequence/acknowledgment numbers, and following TCP streams).

> ⚠️ **Disclaimer:** All packet analysis exercises are conducted strictly for educational and authorized training purposes within simulated lab environments.

---

## ⚙️ Environment & Tooling Summary

| Component | Specification / Setting |
| :--- | :--- |
| **Primary Tool** | Wireshark Network Protocol Analyzer |
| **Analyzed Protocols** | Ethernet, IPv4, TCP, UDP, DNS, HTTP |
| **Analysis Platform** | Cross-platform trace file review & packet dissection |
| **Documentation Format** | Markdown (`README.md`) structured per lab module |

---

## 📂 Lab Directory Structure

* **[Lab 1: Introduction to Wireshark & Basic Filtering](./Lab-1-Basics/)**
  * Live capture and trace file loading.
  * Protocol dissection across OSI layers.
  * Filtering traffic using source/destination IPs and protocols (`ip.addr`, `dns`, `http`).

* **[Lab 2: TCP Handshake & Traffic Analysis](./Lab-2-TCP-Analysis/)**
  * Step-by-step examination of the 3-way handshake (`SYN`, `SYN-ACK`, `ACK`).
  * Tracking sequence numbers, acknowledgment numbers, and TCP flags (`RST`, `FIN`).
  * Reconstructing application sessions using the **Follow TCP Stream** tool.

---

## 🛠️ Key Wireshark Filters Practiced

- **Host Isolation:** `ip.addr == <IP_ADDRESS>` — Isolates all traffic to/from a specific host.
- **Web Traffic:** `tcp.port == 80 || tcp.port == 443` — Filters standard web traffic.
- **DNS Lookup:** `dns` — Captures Domain Name System queries and responses.
- **SYN Scans & Open Ports:** `tcp.flags.syn == 1 && tcp.flags.ack == 1` — Identifies server responses / open ports.
- **Closed Ports:** `tcp.flags.reset == 1` — Isolates connection resets and closed ports.

---

## 💡 What I Learned

Through these practical labs, I developed a deeper understanding of packet-level network behaviors. Key takeaways include:
1. **Packet Structure & Dissection:** Reading raw headers to understand how data moves across layers of the OSI model.
2. **Display Filtering:** Using efficient filter expressions to quickly weed out noise and isolate relevant investigation targets.
3. **TCP Connection States:** Tracking handshake integrity, retransmissions, flags, and graceful vs. forced connection teardowns.
4. **Security Visibility:** Recognizing basic network baseline patterns versus scanning or anomalous behaviors.
5. **Technical Documentation:** Maintaining clean, structured GitHub repositories to showcase technical competencies.

---

## 🔗 Tools & Resources

- **Wireshark Official Downloads:** [https://www.wireshark.org/download.html](https://www.wireshark.org/download.html)
- **NetworkWalks Training Material & Scenarios**

---

## 👤 Author

**Malek Aroua**  
*Computer Networks Graduate | Cybersecurity Specialist*  

---
*Project completed as part of the NetworkWalks Cybersecurity Certification Program.*
