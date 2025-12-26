# 🔎 SOC Assessment Notes – HTTP Log Analysis (Splunk SIEM)

---

## 🎯 Assessment Objective

This assessment was performed to simulate a **SOC analyst workflow** for analyzing HTTP access logs using Splunk SIEM. The focus of the exercise was to understand how raw web server logs are ingested, parsed, and analyzed to identify abnormal behavior and security-relevant patterns.

The assessment emphasizes **log onboarding, field extraction, and analyst-driven investigation**, rather than real-time alerting or exploitation.

---

## 🧪 Assessment Scope

✔ Manual ingestion of HTTP access logs  
✔ Source type and index configuration  
✔ Regex-based field extraction  
✔ SPL-based traffic analysis  
✔ Error and anomaly investigation  
✔ Suspicious source identification  

❌ No forwarders  
❌ No live traffic  
❌ No dashboards  
❌ No automated alerts  
❌ No attack simulation  

---

## 📥 Log Ingestion Methodology

Sample HTTP access logs were prepared in text format and uploaded into Splunk using the web interface.

**Ingestion Method**
- Splunk Web → *Settings → Add Data → Upload*

**Validation Steps**
- Confirmed events were indexed successfully  
- Verified logs were searchable  
- Ensured correct metadata assignment  

This approach mirrors how analysts often ingest historical or offline log data during investigations.

---

## ⚙️ Source Type & Index Handling

During ingestion:
- An HTTP-appropriate sourcetype was selected  
- Index and host values were reviewed  
- Configuration was validated before submission  

Correct sourcetype selection ensured **consistent parsing and reliable SPL querying**.

---

## 🧱 Field Extraction Strategy

Manual field extraction was performed using Splunk’s **Extract New Fields** feature with regular expressions.

Fields extracted included:
- Source IP  
- Destination IP  
- Request method  
- HTTP status  
- Status code  
- Source port  
- Destination port  

This step transformed unstructured log data into **structured, query-ready fields**.

---

## 🧠 Analyst Perspective

This assessment reinforces the importance of:
- Understanding data before detection  
- Prioritizing accuracy over automation  
- Applying analyst judgment when interpreting anomalies  

---

## 📌 Documentation Purpose

This document demonstrates **SOC-aligned log ingestion, parsing, and analysis methodology**, consistent with blue-team monitoring practices.
