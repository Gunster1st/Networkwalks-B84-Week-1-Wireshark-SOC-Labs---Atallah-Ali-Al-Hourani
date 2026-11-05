# Networkwalks-B84-Week-1-Wireshark-SOC-Labs---Atallah-Ali-Al-Hourani
Hands-on network security, traffic analysis, and protocol inspection labs completed using Wireshark, covering FTP brute-force detection and VoIP/SIP/RTP analysis.

# 🛡️ Network Security & Traffic Analysis Labs (Wireshark)

This repository documents my hands-on investigations and labs focused on network traffic analysis, protocol inspection, and security monitoring using **Wireshark**. All labs were completed successfully with a **100% score (NO hints used)**.

---

## 🚀 Skills & Techniques Mastered

### 1. Brute-Force Attack Analysis (Lab 7)
* **Attack Vector Isolation:** Used display filters (such as `ftp.response.code == 530` and `ftp.response.code == 230`) to isolate failed login attempts from successful sessions.
* **Credential Discovery:** Analyzed plain-text control channels to identify attacker usernames, password guesses, and successful authentication tokens (`PASS`).
* **SOC Investigation Mindset:** Tracked exact request-response sequences to reconstruct unauthorized access events.

### 2. VoIP & SIP Signaling Analysis (Lab 8)
* **Protocol Segregation:** Differentiated between signaling traffic (**SIP**) and audio media streams (**RTP**).
* **Call Flow Reconstruction:** Filtered and inspected session initiation messages (`INVITE`, `100 Trying`, `180 Ringing`, `200 OK`) to identify callers, recipients, and extension numbers.
* **Media Codec Inspection:** Analyzed RTP payload types (**PCMU / G.711**) and evaluated mitigation strategies against eavesdropping (e.g., implementing **SRTP** for encrypted voice communications).

---

## 📸 Lab Evidence & Screenshots

### 🔑 FTP Brute-Force Detection
*Isolating failed login responses and tracking down the successful authentication:*
![FTP Brute Force Analysis](screenshots/image_9c57e3.jpg)

### 📞 VoIP / SIP Call Setup
*Tracing SIP session initiation headers and extension details:*
![SIP Protocol Analysis](screenshots/image_9bf2e0.jpg)

### 🔊 RTP Audio Packet Analysis
*Inspecting G.711 PCMU voice codecs:*
![RTP Traffic Analysis](screenshots/image_9beb41.jpg)

---

## 🛠️ Tools Used
* **Wireshark** (Packet Capture & Protocol Analysis)
* **TCP/IP Stack & UDP/TCP Protocols**
* **FTP & SIP/RTP Protocol Suites**

---
*Completed as part of practical network security training.*
