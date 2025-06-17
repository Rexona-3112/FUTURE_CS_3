# 🔐 Wi-Fi Security Assessment | Task 3 - Future Interns

This repository contains the deliverables for **Task 3** of my internship under the **Future Interns** program. The task involved conducting a **Wi-Fi security assessment** using industry-standard tools such as **Wireshark** and **Nmap**, followed by creating a professional report based on the findings.

---

## 🧠 Objective

To evaluate the security posture of a home Wi-Fi network by:
- Capturing and analyzing live packet data
- Identifying network protocols in use
- Detecting potential vulnerabilities
- Scanning the local subnet for active devices and open ports

---

## 🛠 Tools Used

- [Wireshark](https://www.wireshark.org/): For capturing and analyzing real-time network traffic.
- [Nmap](https://nmap.org/): For scanning the network and identifying open ports, active hosts, and exposed services.
- Kali Linux Terminal: For running network commands and executing scans.

---

## 🧪 Methodology

### 🔹 Wireshark Analysis
- Captured traffic on the `wlan0` wireless interface.
- Analyzed protocols: `DNS`, `HTTPS`, `HTTP`, `ARP`, `ICMPv6`, and `TCP`.
- Applied filters like `http`, `dns`, `tcp.port==80`, and `tcp.port==443`.
- Extracted conversation statistics and plotted I/O graphs to identify spikes, anomalies, or retransmissions.

### 🔹 Nmap Scanning
- Identified the network range: `192.168.233.0/24`
- Scanned the subnet to find live hosts and exposed services.
- Used both standard and stealth scanning techniques:
  ```
  nmap -sS -sV 192.168.233.0/24
  nmap -Pn -T4 -sS 192.168.233.0/24

---

## 📄 Deliverables

  A full security audit report that includes:

  * Screenshot evidence from Wireshark and Nmap
  * Technical analysis and observations
  * Findings and recommendations
  * Summary of network security posture

---

## 📚 What I Learned

* How to capture and analyze network traffic securely
* Interpreting protocol-level data and filtering sensitive communication
* Using Nmap effectively for internal scanning and reconnaissance
* Identifying threats like open services, DNS leaks, or unencrypted traffic
* Writing structured, evidence-based security reports

---


## 🔐 Recommendations for Home Network Security

* Use WPA2/WPA3 encryption on all routers
* Avoid insecure protocols like HTTP, Telnet, or FTP
* Disable unused services and ports
* Monitor outbound connections and suspicious DNS lookups
* Perform regular packet captures for proactive monitoring

---

## 📌 Author

**Shayan**
Cybersecurity Intern – Future Interns
Date: 17/06/2025

---

## 📢 License

This project is for **educational and learning purposes** only.

---
