#  EDR + SOAR Automation Project

## 📌 Overview
This project demonstrates automated incident detection and response using LimaCharlie (EDR) and Tines (SOAR).

---

## 🧠 Architecture
![Architecture](screenshots/architecture.png)

---

## ⚙️ Workflow
1. Detect suspicious process (LaZagne)
2. Send alert to Tines
3. Automatically isolate machine
4. Notify via Slack & Email

---

## 🛠️ Tech Stack
- LimaCharlie (EDR)
- Tines (SOAR)
- Slack API
- Email (SMTP)

---

## 📸 Demo

### 🛑 Detection
![Detection](screenshots/Detection_Rule1.png)

![Detection](screenshots/Detection_Rule2.png)

Detects execution of LaZagne credential dumping tool using LimaCharlie detection rule.

### ⚙️ Automation (Tines)
![Tines](screenshots/Tines_Workflow.png)

Helps in Automating the entire workflow using Playbooks(stories).
### 🔒 Isolation
![Isolation](screenshots/Isolation_Status.png)
Isolation status of the infected VM in Lima Charlie
### 🔔 Alerts
Alerts sent to the analyst as part of the automation
![Slack](screenshots/slack_message.png)
![Email](screenshots/email_msg.png)

---

## 🎯 Key Features
- Automated threat detection
- Endpoint isolation
- Real-time alerting
- End-to-end SOC workflow

---

## 🚀 Future Improvements
- Add SIEM integration (Splunk/Sentinel)
- Add threat intelligence enrichment
- Reduce false positives with better rules# EDR-SOAR Automation Project (LimaCharlie + Tines)

## Detection Logic

Custom detection rule identifies:
- LaZagne executable
- Suspicious command-line usage
- Known malicious hash
This helps reduce false positives and improves detection accuracy.
