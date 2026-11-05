# Networkwalks-B84-Week-1-Wireshark-SOC-Labs---Atallah-Ali-Al-Hourani
Hands-on network security, traffic analysis, and protocol inspection labs completed using Wireshark, covering FTP brute-force detection and VoIP/SIP/RTP analysis.

<div align="center">

# 🛡️ Network Security & Traffic Analysis Labs

<p align="center">
  <img src="https://img.shields.io/badge/Wireshark-SOC_Lab-1681B0?style=for-the-badge&logo=wireshark&logoColor=white" alt="Wireshark">
  <img src="https://img.shields.io/badge/Score-100%25_(No_Hints)-2ea44f?style=for-the-badge&logo=githubactions&logoColor=white" alt="Score">
  <img src="https://img.shields.io/badge/Protocols-FTP_|_SIP_|_RTP-orange?style=for-the-badge" alt="Protocols">
</p>

*Hands-on network investigations, brute-force analysis, and VoIP traffic inspection completed with absolute precision.*

</div>

---

## 🧭 Executive Summary

This repository houses comprehensive documentation and deep-dive packet analysis from advanced network security labs. Every scenario was investigated from a Security Operations Center (SOC) perspective—isolating attack vectors, decoding session initiation signaling, and validating network hardening measures—achieving a **100% score without relying on hints**.

---

## 🔬 Core Investigations & Methodologies

<table width="100%">
  <tr>
    <td width="50%" valign="top">
      <h3>🔐 Lab 7: FTP Brute-Force Detection</h3>
      <ul>
        <li><b>Attack Vector Isolation:</b> Applied specific display filters (<code>ftp.response.code == 530</code>) to track failed login storms.</li>
        <li><b>Credential Recovery:</b> Traced clear-text control channels through <code>USER</code> and <code>PASS</code> requests.</li>
        <li><b>Access Verification:</b> Pinpointed the exact packet returning <code>230 Login successful</code> and isolated the compromised credential (<code>Sunshine99</code>).</li>
      </ul>
    </td>
    <td width="50%" valign="top">
      <h3>📞 Lab 8: VoIP & SIP Signaling Analysis</h3>
      <ul>
        <li><b>Protocol Segregation:</b> Differentiated between control plane signaling (<b>SIP</b>) and media transport streams (<b>RTP</b>).</li>
        <li><b>Call Flow Reconstruction:</b> Inspected session initiation headers (<code>INVITE</code>, <code>100 Trying</code>, <code>180 Ringing</code>, <code>200 OK</code>).</li>
        <li><b>Codec Inspection & Mitigations:</b> Analyzed <b>PCMU / G.711</b> audio payload types and evaluated **SRTP** encryption for eavesdropping prevention.</li>
      </ul>
    </td>
  </tr>
</table>

---

## 🛠️ Technology Stack & Protocols

* **Analysis Tool:** Wireshark
* **Network Protocols:** TCP, UDP, FTP, SIP (Session Initiation Protocol), RTP (Real-time Transport Protocol), ARP, DNS
* **Security Concepts:** Brute-force detection, credential harvesting, voice stream decryption risks, SRTP implementation

---

## 📁 Repository Structure

```text
├── screenshots/         # Contains step-by-step lab completion visual evidence
└── README.md            # Project documentation and summary
