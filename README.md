# 🛡️ PyIDS  
A custom GUI-based Network Intrusion Detection System (NIDS) written in Python.  
It supports live packet capturing, signature-based alerting, decoded payload viewing, and TCP/HTTP2 stream following.

---

## 💡 FEATURES  
🔸 Live network packet capturing using Scapy  
🔸 Signature-based alerting using rules.txt  
🔸 GUI built with PySimpleGUI  
🔸 View and decode payloads of suspicious packets  
🔸 Save suspicious packets to .pcap  
🔸 Follow HTTP2 and TLS/TCP streams  
🔸 SSL/TLS decryption via key log file (`ssl1.log`)

---

## ⚙️ REQUIREMENTS  
• Python 3.8+  
• scapy  
• pyshark  
• PySimpleGUI  
• Wireshark/tshark (for HTTP2/TLS support)

**Install using:**  
`pip install scapy pyshark PySimpleGUI`  

**Run:**  
Run `custom_ids.py` as administrator.  
Ensure `savedpcap/` and `temp/` folders exist.

---

## 🕹️ USAGE (GUI BUTTONS)  
**STARTCAP** → Start capturing traffic  
**STOPCAP** → Stop capturing  
**SAVE ALERT** → Save flagged packets to `savedpcap/`  
**REFRESH RULES** → Reload rules from `rules.txt`  
**ALERT PACKETS** → View flagged packets (left panel)  
**ALL PACKETS** → View all captured packets (right panel)  
**ALERT DECODED** → View decoded payloads for alerts  
**TCP STREAMS** → View TCP streams (select to inspect)  
**HTTP2 STREAMS** → View HTTP2 streams  
**HTTP OBJECTS** → Extract objects from HTTP streams.
