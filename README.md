Udhar Reminder System

An automated payment reminder system built using **n8n**, **Google Sheets**, and **WhatsApp Cloud API**. The workflow automatically identifies overdue payments from a Google Sheet, sends WhatsApp reminders to customers, and updates the reminder status to avoid duplicate notifications.



Project Overview

Managing udhar (credit) payments manually can be time-consuming and error-prone. This project automates the reminder process by:

- Reading customer payment records from Google Sheets
- Checking whether the due date has passed
- Sending automated WhatsApp reminders
- Updating the reminder status in the sheet
- Running automatically on a schedule using n8n



Features

- Automated workflow using n8n
- Google Sheets integration
- WhatsApp Cloud API integration
- Scheduled reminder execution
- Due-date validation
- Automatic status updates
- Scalable for multiple customers
- No manual follow-up required



Tech Stack

| Technology | Purpose |
|------------|---------|
| n8n | Workflow Automation |
| Google Sheets API | Data Storage |
| WhatsApp Cloud API | Sending Notifications |
| Meta Graph API | WhatsApp Messaging |
| JavaScript Expressions | Workflow Logic |

---
Workflow Architecture


Schedule Trigger
       │
       ▼
Get Rows from Google Sheet
       │
       ▼
Check Due Date (IF Node)
       │
       ▼
Loop Over Due Records
       │
       ▼
Send WhatsApp Reminder
       │
       ▼
Update Status in Sheet

Project Structure

Udhar-Reminder-System/
│
├── README.md
├── workflow.json
└── screenshots
   
Sample Data

| ID | Name | Phone Number | Amount | Due Date | Status |
|----|------|--------------|---------|----------|---------|
| 1 | Rahul | 919999999999 | 500 | 2026-05-01 | pending |

---

## 💬 Sample Reminder Message

Hello Rahul,

This is a reminder that your payment of ₹500 is overdue.

Due Date: 01-May-2026

Please make the payment at your earliest convenience.

Thank you.


Setup Instructions

1. Import Workflow

- Open n8n
- Click **Import Workflow**
- Upload `workflow.json`

2. Configure Google Sheets

- Create Google Sheets credentials
- Connect your sheet
- Update the Sheet ID if required

3. Configure WhatsApp Cloud API

- Create a Meta Developer App
- Enable WhatsApp Cloud API
- Generate an Access Token
- Configure credentials in n8n

4. Activate Workflow

- Enable the Schedule Trigger
- Activate the workflow
- Test by adding sample  

Learning Outcomes

Through this project, I gained practical experience in:

- Workflow Automation
- API Integration
- WhatsApp Cloud API
- Google Sheets Automation
- No-Code / Low-Code Development
- Process Automation
- Business Workflow Design

Future Enhancements

- Payment links in reminders
- Add a google form
- Dashboard and analytics
- Reminder frequency customization




Skills Demonstrated

- SQL
- Data Analysis
- Workflow Automation
- API Integration
- Google Sheets
- n8n
- Problem Solving



