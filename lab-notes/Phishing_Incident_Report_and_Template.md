
## 🛡️ Incident Report: Phishing Email Investigation

### 📌 Incident Summary:
A phishing alert was generated from email logs showing suspicious links sent to multiple users. The subject line and sender domain matched known phishing campaigns.

### 🕒 Date/Time Identified:
June 10, 2025, 10:24 AM EST

### 🧰 Tools Used:
- Splunk
- Wireshark
- VirusTotal

### 🔍 Indicators of Compromise (IOCs):
- **Sender:** accounts@support365.com
- **Subject:** "Update your account credentials"
- **URL:** hxxps://secure-login365[.]info
- **Affected Users:** 3 (confirmed click-throughs)

### 📚 Log Sources:
- Email gateway logs (via Splunk)
- Firewall logs (outbound connections)

### ✅ Actions Taken:
- Blocked domain at firewall and proxy
- Quarantined emails in user inboxes
- Initiated password reset for affected accounts
- Searched Splunk for lateral movement and failed logins

### ⏭️ Next Steps:
- Update phishing awareness training
- Add domain to blocklist
- Monitor affected accounts for 72 hours before closing

---

## 📣 Escalation Message Example

**Subject:** Escalation – Confirmed Phishing Incident with Credential Compromise

**Summary:**  
A phishing email was received by 3 users. At least one user submitted credentials on a spoofed login page.

**Actions Taken:**  
- Domain blocked  
- Users contacted  
- Passwords reset

**Request:**  
Please review affected accounts for unusual access and determine if legal/compliance needs to be notified.

---

## 🧾 Blank Template for Future Investigations

### Incident Summary:
[Write a short paragraph summarizing what happened]

### Date/Time Identified:
[Insert time and date]

### Tools Used:
- [Example: Splunk, Wireshark, CrowdStrike]

### Indicators of Compromise (IOCs):
- Sender:
- Subject:
- URL/IP:
- Affected Users:

### Log Sources:
- [e.g., Email logs, Endpoint logs, Authentication logs]

### Actions Taken:
- [List step-by-step actions]

### Next Steps:
- [Post-incident improvements, awareness training, etc.]

### Escalation Message:
- [Draft a short formal message to escalate to another team]

