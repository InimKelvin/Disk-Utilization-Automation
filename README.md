# 💾 Disk Utilization Management Automation

**Tool**: Power Automate  
**Domain**: IT Operations  
**Focus**: Proactive Resource Monitoring

---

## 📘 Project Overview

This project utilizes **Microsoft Power Automate** to automate server disk space monitoring. It processes incoming disk usage reports from Outlook, filters for servers exceeding a **70% disk utilization threshold**, and sends **personalized alert emails** to each server owner listing only their affected servers.

The automation reduces manual workload, ensures timely notifications, and enhances infrastructure reliability.

---

## 🛠️ Tools & Technologies

- **Power Automate** – Workflow automation
- **Outlook** – Email reports (Excel attachments)
- **Excel Online (Business)** – Data parsing and transformation
- **Office 365 Mail** – Sending customized alert emails

---

## 🔄 Workflow Description

### 1️⃣ Trigger – Email Attachment Monitoring
- Flow is triggered by the arrival of a scheduled report via Outlook.
- The email contains an Excel attachment with server disk utilization data.

### 2️⃣ Data Filtering & Grouping
- The Excel file is parsed using Excel Online.
- Rows where `Disk Usage % > 70` are filtered.
- Filtered data is grouped by `Server Owner`.

### 3️⃣ Personalized Reporting
- Each owner receives an email with:
  - A dynamic table of their affected servers
  - Disk usage percentage per server
  - A personalized greeting and action note

📸 [View Flow Diagram](https://github.com/InimKelvin/Disk-Utilization-Automation/blob/main/assets/disk_utilization_flow.png)

---

## 📊 Results & Metrics

| Metric | Value |
|--------|-------|
| ⏱️ Manual Time Saved | ~30 minutes/day (~10 hours/month) |
| 📬 Emails Sent | Up to 20 personalized emails per run |
| 🚨 Threshold | 70% Disk Utilization |
| ✅ Error Reduction | 100% decrease in manual reporting errors |
| 🔁 Frequency | Automated daily or per report |

---

## ✅ Benefits

- 📈 **Scalable** – Handles any number of records and users
- 📨 **Targeted Alerts** – Each owner gets only relevant information
- ⚡ **Faster Notifications** – Triggered instantly on report arrival
- 📊 **Reliable Reporting** – No missed or outdated alerts
- 🔧 **Maintainable** – Easy to update threshold or logic in the flow

---

## 🔍 Conclusion

This project showcases the power of **Power Automate** in IT operations. It transforms a manual reporting task into a fully automated process that ensures consistent and proactive monitoring of server disk space.

> **Note**: Only sanitized screenshots are included in this repository. The actual Power Automate flow export is excluded to avoid sharing sensitive organizational configurations.


---


