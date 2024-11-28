# EC3_REU
# IoT Vulnerabilities and Cybersecurity Research

## Overview
This repository contains my research conducted over the summer at Sonoma State University with EC3, funded by the National Science Foundation. 
The project investigates vulnerabilities in IoT devices, particularly wireless-connected cameras, and their associated networks. Through simulated 
Denial of Service (DoS) attacks, we expose security loopholes these devices could present.

### Key Objectives
- Explore the vulnerabilities in WPA2-PSK networks used by IoT devices.
- Conduct network reconnaissance, four-way handshake capture, password decryption, traffic decryption, and MAC spoofing.
- Propose layered security measures to mitigate IoT-related vulnerabilities.

---

## Contents
- **[Poster](poster/)**: A concise visual representation of the research.
- **[Paper](paper/)**: In-depth analysis and findings.
- **[Code](code/)**: Programs created to monitor and provide alerts for LAN security.

---

## Findings
The study highlights the ease of cracking WPA2-PSK networks and the critical need for enhanced security, including:
- Modern encryption protocols
- Unique and longer passwords or certificate-based authentication
- Intrusion detection and prevention systems
- Implementation of 802.11w

---

## Programs
The `code/` directory contains:
- **New_Device_Detector**: This Python script uses Scapy to sniff for Wi-Fi probe requests
  on a given network interface, and displays any new devices it detects in a Tkinter window.
  It identifies devices by their MAC addresses, and also displays the SSID from the probe
  requests when available.
- **Lan_Monitor**: This Python script is a simple network monitor tool that uses the ICMP
  protocol to continuously ping a pre-defined set of hosts in your Local Area Network (LAN).
- **Deauth_Detector**: This is a script for a simple Deauthentication (Deauth) Attack
  Detector that uses Scapy to sniff network traffic for Deauth packets, an indicator of a
  Deauth attack. The script provides a graphical user interface (GUI) using Tkinter, where
  the state of the network is displayed. The status changes from 'Secure' to 'Deauth attack
  in progress' based on the detection of Deauth packets.
- **Arduino_Camera_Web_Server**: This repository contains an example application for an
  ESP32-based camera server. The program configures the ESP32 to capture images using a
  camera module, and streams them over WiFi to a web browser UI. This builds off of the
  example web server project in the Arduino IDE.

---



## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
