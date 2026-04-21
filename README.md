# 🔍 Wireshark Network Traffic Analysis

## 📌 Project Overview

This project demonstrates a practical network traffic analysis using Wireshark.
The goal is to analyze captured packets and extract meaningful insights about user activity, communication patterns, and protocol behavior.

---

## 🧪 Analysis Performed

### 🔹 DNS Analysis

The DNS traffic reveals that the user queried multiple domains, including:

* youtube.com
* google-analytics.com
* googletagmanager.com

This confirms domain resolution activity and allows mapping domain names to IP addresses.

📸 *Screenshot: DNS query showing youtube.com*

---

### 🔹 TCP Analysis

TCP packets were analyzed to understand connection behavior.

* SYN and ACK flags were observed
* Sequence and Acknowledgment numbers were analyzed
* TCP communication flow was successfully interpreted

Note: The full TCP 3-way handshake was not captured, as it occurred before the capture started.

📸 *Screenshot: TCP packet with SYN and ACK flags*

---

### 🔹 HTTP Analysis

Unencrypted HTTP traffic was successfully captured and analyzed.

* HTTP GET requests were observed
* Server responses with **200 OK** status were identified
* Full request URI was extracted

Example:

* `GET / HTTP/1.1`
* `HTTP/1.1 200 OK`

📸 *Screenshot: HTTP request and response details*

---

### 🔹 TLS (HTTPS) Analysis

Encrypted traffic was analyzed using TLS protocol inspection.

* TLS Client Hello packets were identified
* Server Name Indication (SNI) field revealed accessed domains

Example domains:

* insecure.org
* nmap.org

This demonstrates the ability to identify user activity even in encrypted traffic.

📸 *Screenshot: TLS Client Hello with SNI field*

---

### 🔹 Traffic & IP Analysis (Conversations)

Using the **Statistics → Conversations** feature:

* The most active IP addresses were identified
* Data transfer volume (bytes) was analyzed
* Communication patterns between hosts were examined

This helps determine the most significant network interactions.

📸 *Screenshot: Conversations showing highest data exchange*

---

## 🧠 Key Findings

* The user performed normal web browsing activity
* DNS, TCP, HTTP, and TLS protocols behaved as expected
* No suspicious or malicious traffic patterns were detected
* Encrypted and unencrypted traffic were both successfully analyzed

---

## 📂 Project Structure

* `capture.pcap` → Network traffic capture file
* `screenshots/` → Wireshark analysis screenshots
* `README.md` → Project documentation

---

## 🚀 Skills Demonstrated

* Packet-level network analysis
* Protocol inspection (DNS, TCP, HTTP, TLS)
* Traffic behavior interpretation
* Identifying domains from encrypted traffic (SNI analysis)
* Network conversation and flow analysis

---

## 🎯 Conclusion

This project showcases the ability to:

* Analyze real network traffic using Wireshark
* Interpret communication between systems
* Extract meaningful insights from packet data

It reflects practical skills relevant to roles such as:

* SOC Analyst
* Network Security Analyst
* Junior Cybersecurity Analyst

---
