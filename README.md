# 🔍 Network Traffic Analysis with Wireshark

## 📌 Overview

This project presents a structured network traffic analysis performed using Wireshark.
The objective is to inspect captured packets, identify communication patterns, and interpret protocol behavior across multiple layers of the network stack.

---

## 🧪 Methodology

The analysis was conducted using a layered approach:

1. Domain resolution analysis (DNS)
2. Connection behavior inspection (TCP)
3. Application layer inspection (HTTP)
4. Encrypted traffic analysis (TLS)
5. Traffic flow and communication analysis (Conversations)

---

## 🔎 Analysis Details

### 🔹 DNS Analysis

DNS traffic was examined to identify domain resolution activity.

Observed domains include:

* youtube.com
* google-analytics.com
* googletagmanager.com

This confirms that user activity triggered domain-to-IP resolution through DNS queries.

---

### 🔹 TCP Analysis

TCP packets were analyzed to understand connection behavior and reliability.

Key observations:

* SYN and ACK flags were identified
* Sequence and Acknowledgment numbers were examined
* TCP communication flow was interpreted successfully

> Note: The full TCP 3-way handshake was not captured, as it occurred prior to the start of packet capture.

---

### 🔹 HTTP Analysis

Unencrypted HTTP traffic was captured and analyzed.

Findings:

* HTTP GET requests were observed
* Server responses returned **200 OK** status
* Full Request URI was successfully identified

This demonstrates visibility into application-layer communication.

---

### 🔹 TLS (HTTPS) Analysis

Encrypted traffic was analyzed using TLS protocol inspection.

Key findings:

* TLS Client Hello packets were identified
* Server Name Indication (SNI) revealed accessed domains

Observed domains:

* insecure.org
* nmap.org

This highlights the ability to infer user activity even within encrypted traffic.

---

### 🔹 Traffic & IP Analysis (Conversations)

Traffic patterns were analyzed using Wireshark’s **Conversations** feature.

Insights:

* Most active IP addresses were identified
* Data transfer volume (bytes) was analyzed
* Communication intensity between hosts was evaluated

---

## 🧠 Key Findings

* The captured traffic represents normal user web activity
* DNS, TCP, HTTP, and TLS protocols operated as expected
* No anomalous or suspicious behavior was detected
* Both encrypted and unencrypted traffic were successfully analyzed

---

## 📂 Project Structure

```id="djnjqd"
wireshark-traffic-analysis/
│
├── capture.pcap
├── screenshots.png
├── README.md
```

---

## 🛠️ Tools & Technologies

* Wireshark
* TCP/IP Protocol Suite
* DNS, HTTP, TLS

---

## 🚀 Skills Demonstrated

* Network traffic analysis
* Packet-level inspection
* Protocol analysis (DNS, TCP, HTTP, TLS)
* Encrypted traffic interpretation (SNI analysis)
* Identifying communication patterns and active hosts

---

## 🎯 Conclusion

This project demonstrates the ability to analyze real network traffic and extract meaningful insights from packet data.

It reflects practical, hands-on skills relevant to roles such as:

* SOC Analyst
* Network Security Analyst
* Junior Cybersecurity Analyst

---

