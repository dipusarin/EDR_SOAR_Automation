# EDR-SOAR Automation Project (LimaCharlie + Tines)

## 📌 Overview
This project demonstrates an automated Security Operations (SOAR) workflow integrating an EDR platform with automation and response capabilities.

## ⚙️ Technologies Used
- LimaCharlie (EDR)
- Tines (SOAR)
- Slack (Alerting)
- Email Notifications

## 🚀 Workflow

1. Detection triggered in LimaCharlie (LaZagne execution)
2. Webhook sends event to Tines
3. User prompt asks analyst for action
4. If approved:
   - Host is isolated via API
5. Alerts sent to Slack and Email

## 🔍 Detection Logic
Custom detection rule for LaZagne based on:
- File path
- Command line
- Parent process
- Known hash

## 🛡️ Response Actions
- Host isolation via LimaCharlie API
- Real-time alerting
- Human-in-the-loop decision making

## 📸 Screenshots
See `/screenshots` folder for:
- Detection rule
- Tines workflow
- Slack alerts
- Isolation confirmation

## 🧠 Key Learnings
- EDR + SOAR integration
- Detection engineering
- API-based response automation
- Reducing false positives

## 🔮 Future Improvements
- Add Mimikatz detection
- Integrate VirusTotal enrichment
- Automate severity scoring

## Architecture Diagram

This diagram shows the flow between LimaCharlie, Tines, Slack, and Email alerts.
![Architecture](screenshots/architecture.png)


##  Demo 

### Detection in LimaCharlie
![Detection](screenshots/Detection_Rule1.png)

![Detection](screenshots/Detection_Rule2.png)

### Tines Workflow Execution
![Tines](screenshots/Tines_Workflow.png)

### Slack Alert
![Slack](screenshots/slack_message.png)

### Email Notification
![Email](screenshots/email_msg.png)
