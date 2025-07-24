# Analyze-network-attacks

## 📘 Overview

This repository contains a hands-on cybersecurity investigation activity. You will examine a Wireshark-captured network log to identify and analyze a suspected network attack that caused a service interruption for a customer accessing the company website.

Using the log file and knowledge of network attacks, you will determine the type of attack, how it occurred, and the impact it had on the organization. A completed **Cybersecurity Incident Report** is provided for reference.

---

## 🧠 Scenario Summary

A customer experienced issues accessing the company’s website. As a cybersecurity analyst, you are assigned to:

1. Analyze Wireshark traffic logs for suspicious or malicious behavior.
2. Identify the likely cause of the incident.
3. Determine how the attack was executed.
4. Describe the negative impact on the website and organization.
5. Document the incident findings in a professional report.

---

## 📂 Repository Contents

| File/Folder | Description |
|-------------|-------------|
| `logs/` | Contains Wireshark log file (`.pcap` or `.csv` format) captured during the attack. |
| `Cybersecurity_Incident_Report.pdf` | A sample report outlining the incident analysis, findings, and recommendations. |

---

## 🧰 Tools Required

- [Wireshark](https://www.wireshark.org/) – To open and analyze `.pcap` logs.
- Spreadsheet software or Python (optional) – For parsing `.csv` logs if applicable.

---

## 🎯 Learning Objectives

By completing this activity, you will learn how to:

- Use Wireshark to analyze network traffic.
- Identify signs of common attacks (e.g., DDoS, DNS amplification, port scanning).
- Trace attack patterns and malicious IPs.
- Document cybersecurity incidents with evidence and impact analysis.

---

## 🔍 How to Complete the Exercise


1. **Analyze the Attack**
   - Identify the attack vector (e.g. DNS attack, DoS, brute force).
   - Determine the attacker’s source IP (if available).
   - Document packet patterns, timestamps, and payload anomalies.

2. **Review or Write the Report**
   - Compare your analysis with the `Cybersecurity_Incident_Report.pdf`.
   - If desired, draft your own version before reviewing the sample report.

---

## 🔁 Common Wireshark Filters

```wireshark
http
dns
icmp
tcp.port == 80
ip.addr == x.x.x.x
udp.port == 53
frame contains "malicious-domain.com"
