# 🔎 HTTP Log Analysis & Anomaly Detection using Splunk SIEM

This project demonstrates a **Security Operations (SOC)-style analysis of HTTP server logs using Splunk SIEM**, focused on identifying abnormal behavior, suspicious patterns, and potential security incidents.

The objective of this project is to simulate how a SOC analyst ingests logs, builds searches, detects anomalies, and interprets security-relevant events from web traffic.

---

## 🎯 Project Objective

The primary goal of this project is to:

- Analyze HTTP server logs using Splunk SIEM  
- Identify anomalous or suspicious request patterns  
- Detect potential attack indicators  
- Understand web traffic behavior  
- Practice log-driven investigation workflows  
- Strengthen SOC-level monitoring and analysis skills  

This project focuses on **detection and analysis**, not exploitation.

---

## 🧪 Environment Overview

| Component | Description |
|--------|-------------|
| SIEM Platform | Splunk Enterprise |
| Log Source | HTTP access logs |
| Data Type | Web traffic / application logs |
| Analysis Type | Detection & anomaly analysis |
| Use Case | SOC monitoring & investigation |

---

## 📂 Data Ingestion Overview

HTTP log files were ingested into Splunk using file-based ingestion.  
Once indexed, logs were parsed and analyzed to extract meaningful security signals.

### Key Fields Analyzed
- Client IP address  
- Request method  
- Requested URI  
- HTTP response code  
- User-Agent  
- Timestamp  
- Request frequency  

---

## 🧭 Analysis Workflow

The investigation followed a structured SOC-style workflow:

### 1. Log Ingestion & Verification
- Uploaded HTTP access logs into Splunk  
- Verified indexing and timestamp parsing  
- Ensured searchable fields were extracted  

### 2. Baseline Behavior Analysis
- Observed normal request patterns  
- Identified common endpoints  
- Studied HTTP response distributions  
- Analyzed request frequency trends  

### 3. Anomaly Detection
- Detected unusually high request rates  
- Identified abnormal HTTP methods  
- Flagged suspicious status codes  
- Observed irregular user-agent strings  
- Detected repeated failed requests  

### 4. Threat-Oriented Analysis
- Potential brute-force indicators  
- Scanning behavior patterns  
- Enumeration-like activity  
- Error-based probing attempts  

### 5. Investigation & Interpretation
- Correlated events over time  
- Identified suspicious IP behavior  
- Assessed severity and impact  
- Classified findings logically  

---

## 🔍 Types of Anomalies Analyzed

### Abnormal Request Volume
- Sudden spikes in request count  
- Repeated access from single IPs  
- Traffic bursts inconsistent with baseline  

### Suspicious HTTP Status Codes
- High frequency of 4xx errors  
- Repeated 401 / 403 responses  
- Server-side error patterns (5xx)  

### Malicious Request Patterns
- Repeated probing of endpoints  
- Suspicious URL structures  
- Potential scanning behavior  
- Enumeration-style access  

### User-Agent Anomalies
- Missing or malformed user-agent strings  
- Non-browser identifiers  
- Repeated automated signatures  

---

## 🛠️ Tools & Technologies Used

- **Splunk Enterprise**
- SPL (Search Processing Language)
- HTTP access logs
- Linux environment
- SOC-style log analysis methodology

---

## 📊 Detection Use Cases Implemented

- High-frequency request detection  
- Failed request anomaly detection  
- Suspicious endpoint access  
- Traffic spike identification  
- Abnormal client behavior detection  
- Potential scanning activity recognition  

---

## ⚠️ Ethical Disclaimer

This project was conducted strictly for **educational and defensive purposes** using sample or lab-generated log data.

- No live systems were attacked  
- No unauthorized access occurred  
- No real user data was involved  

---

## 📘 Why This Project Matters

This project demonstrates:

- SOC-level log analysis skills  
- Ability to interpret HTTP logs  
- Understanding of attacker behavior patterns  
- Experience with Splunk searches  
- Detection-driven security thinking  
- Professional documentation practices  

---

📌 *This repository is part of my cybersecurity portfolio and demonstrates hands-on experience with SIEM-based log analysis and anomaly detection.*

