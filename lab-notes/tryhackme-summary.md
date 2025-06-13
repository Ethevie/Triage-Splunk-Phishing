# TryHackMe - SOC Level 1 Lab: Phishing Investigation

## 🧪 Lab Overview
This investigation was done in the Junior Security analyst room on TryHackMe. The goal was to analyze a suspicious phishing alert using Splunk and identify whether it was a true positive or false positive.

## 🔍 Steps Taken
1. Reviewed the alert triggered in Splunk related to a suspicious email.
2. Checked fields like `threat_score`, `geo_location`, `dest_ip`, and `src_email`.
3. Identified that the email originated from a known phishing IP address.
4. Verified the email was a **true positive**.
5. Documented findings and updated dashboard.

## 📊 Splunk Queries Used
```spl
index=phishing_alerts threat_score>70 | table _time, src_email, dest_ip, threat_score, geo_location
