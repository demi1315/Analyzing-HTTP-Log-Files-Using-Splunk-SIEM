# 🔎 SOC Assessment Notes – HTTP Log Analysis (Splunk SIEM)

---

## 🎯 Assessment Objective

This assessment was conducted to **simulate a real-world SOC monitoring scenario**, where HTTP server logs are ingested into a SIEM platform and analyzed to detect **abnormal behavior, potential reconnaissance, and early indicators of attack activity**.

Rather than focusing on exploitation, the goal was to practice **log-driven investigation and analyst decision-making**, which forms the foundation of Security Operations Center (SOC) work.

---

## 🧭 Analyst Workflow Overview

The investigation followed a **SOC-aligned workflow** commonly used in operational environments:

1️⃣ **Log ingestion and validation**  
2️⃣ **Baseline traffic understanding**  
3️⃣ **Anomaly identification**  
4️⃣ **Threat interpretation**  
5️⃣ **Risk context and response consideration**

This mirrors how analysts move from raw telemetry to actionable insight.

---

## 📥 Log Ingestion & Validation

HTTP access logs were ingested into **Splunk Enterprise** using file-based ingestion.

Key validation steps included:
- Ensuring timestamps were parsed correctly  
- Verifying key HTTP fields were extracted  
- Confirming events were searchable and consistent  

This step is critical — **poor ingestion leads to poor detection**.

---

## 📊 Baseline Traffic Analysis

Before flagging anomalies, normal behavior was observed to establish a baseline.

Baseline analysis focused on:
- Typical request volume patterns  
- Common HTTP methods and endpoints  
- Normal response code distribution  
- Expected user-agent behavior  

Understanding “normal” traffic is essential to **avoid false positives**.

---

## 🚨 Anomaly Identification Approach

Once a baseline was established, attention shifted to **deviations**, including:

- Sudden spikes in request volume  
- Repeated requests from a single source  
- Excessive error responses  
- Unusual HTTP methods  
- Irregular or automated user-agent strings  

These signals often represent **early-stage attack activity**.

---

## 🧠 Analyst Interpretation

Not every anomaly is malicious. Each finding was interpreted by asking:

- Is this behavior consistent with legitimate usage?  
- Does it repeat over time?  
- Is it isolated or correlated with other signals?  

This step reflects **analyst judgment**, not blind alerting.

---

## 📝 Purpose of This Document

This document demonstrates:
- SOC-style investigative thinking  
- Structured log analysis methodology  
- Ability to reason about security signals  
- Professional documentation practices  

All analysis was performed using **lab-generated log data for defensive learning purposes**.
