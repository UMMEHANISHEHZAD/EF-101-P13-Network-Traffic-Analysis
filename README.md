# EF-101-P13-Network-Traffic-Analysis
Network traffic observation and analysis project using Wireshark and GitHub (EF101-P13).
# 📌 Project Overview
This project fulfills the requirements for **EF101-P13: Network Traffic Observation and Analysis**. The goal is to analyze, document, and visualize real-time network communications across key application and transport layer protocols using Wireshark and command-line network tools.

---

## 🛠️ Tools & Environment
* **Packet Capture Tool:** Wireshark
* **Command-Line Tools:** `cmd` / `PowerShell` (`ping`, `nslookup`, `ipconfig`, `curl`)
* **Version Control:** GitHub
* **Diagramming Tools:** Draw.io / Lucidchart
---
## 🔬 Executed Experiments

### 1. ICMP Traffic (Ping)
* **Objective:** Test network connectivity and measure round-trip time (RTT).
* **Command Run:** `ping 8.8.8.8`
* **Capture File:** `icmp.pcapng`

### 2. DNS Query & Resolution
* **Objective:** Capture domain name resolution using a DNS server.
* **Command Run:** `nslookup example.com`
* **Capture File:** `dns.pcapng`

### 3. HTTPS Web Traffic
* **Objective:** Observe TCP three-way handshake and encrypted TLS communications over port 443.
* **Capture File:** `http.pcapng`

### 4. File Transfer (TCP Data Segment Analysis)
* **Objective:** Monitor TCP sequence numbers, segment acknowledgments, and data transfers.
* **Capture File:** `tcp.pcapng`

---

## 📊 Summary of Findings
| Protocol | Source IP | Destination IP | Packet Count / Length | Key Observations |
| :--- | :--- | :--- | :--- | :--- |
| **ICMP** | Local IP | `8.8.8.8` | 4 Requests / 4 Replies | Echo Requests/Replies verified RTT network latency. |
| **DNS** | Local IP | Router / DNS | 2 Packets | Standard Query A record to IP resolution. |
| **HTTPS** | Local IP | Web Server IP | Multiple TCP/TLS | TCP 3-Way Handshake (SYN, SYN-ACK, ACK) + TLS Hello. |
| **TCP** | Local IP | Server IP | Segment Stream | High-volume data stream transfer via TCP segments. |

---
