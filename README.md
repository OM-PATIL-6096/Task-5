# Task 5 - Capture and Analyze Network Traffic Using Wireshark

## 📌 Objective
The goal of this task was to **capture live network traffic using Wireshark** and analyze different network protocols to gain hands-on packet analysis skills and protocol awareness.

---

## 🛠 Tools Used
- **Wireshark** (on Kali Linux 2025 x64 - VMware Workstation)

---

## 📑 Steps Performed
1. Installed and launched Wireshark on the active network interface (`eth0`).
2. Started live packet capture.
3. Generated network traffic by browsing websites and sending requests.
4. Stopped the capture after sufficient packets were collected.
5. Applied filters such as:
   - `ocsp` (Online Certificate Status Protocol)
   - `tcp` (Transmission Control Protocol)
6. Analyzed packet details and identified multiple protocols.
7. Saved the capture as a `.pcap` file.

---

## 🔍 Protocols Identified
During the analysis, the following protocols were observed:

1. **OCSP (Online Certificate Status Protocol)**  
   - Used for checking the revocation status of digital certificates.  
   - Seen with multiple request/response packets.

2. **TCP (Transmission Control Protocol)**  
   - Reliable transport protocol.  
   - Three-way handshake (`SYN`, `SYN-ACK`, `ACK`) was observed.  

3. **TLSv1.3 (Transport Layer Security)**  
   - Provides encryption for secure communications.  
   - Packets showed handshake and encrypted application data.

4. **HTTP (HyperText Transfer Protocol)**  
   - Observed over TCP (port 80).  
   - Contains request/response communication.

---

## 📷 Screenshots
- **OCSP Traffic:**  
  ![OCSP Screenshot](screenshots/ocsp.png)

- **TCP + TLS Traffic:**  
  ![TCP Screenshot](screenshots/tcp.png)

*(Replace the image paths with your actual repo image paths.)*

---

## 📂 Deliverables
- Packet capture file: `task5.pcap`  
- README.md (this file)  
- Screenshots of analysis  

---

## ✅ Conclusion
From the packet capture and analysis:  
- Multiple protocols were identified (OCSP, TCP, TLSv1.3, HTTP).  
- The traffic clearly demonstrated **encrypted communication** as well as **basic TCP handshake**.  
- This task enhanced my understanding of **network traffic analysis, filtering, and protocol behavior** using Wireshark.

---
