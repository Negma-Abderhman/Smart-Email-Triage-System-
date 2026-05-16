# 📧 Smart Email Triage System

> 🚀 AI-Powered Email Automation System using n8n

---

## 🌟 Overview


This project builds a smart system that automatically reads and processes incoming emails.

The system uses AI to classify emails and then performs different actions based on their importance.

It helps reduce manual work and keeps the inbox clean and organized.

---


## 📌 What This System Does

- Reads emails from Gmail  
- Classifies emails into categories using AI  
- Performs actions automatically  
- Creates draft replies for urgent emails  
- Archives unimportant emails  
- Logs all activities in Google Sheet

## 🎯 Problem

Managing emails manually leads to:
- Inbox clutter  
- Delayed responses  
- Difficulty prioritizing emails  

---

## 📊 Email Categories

The system classifies emails into four types:

- URGENT → needs immediate action  
- IMPORTANT → normal emails  
- NEWSLETTER → updates or promotions  
- SPAM → unwanted emails  

---


## 🛠 Tech Stack

- n8n  
- Gmail API  
- AI Model  
- Google Sheets  

---

## 🔄 Workflow

1. Fetch emails from Gmail  
2. Classify using AI  
3. Extract data  
4. Route using Switch node  
5. Apply actions:
   - URGENT → Draft reply  
   - IMPORTANT → No action  
   - NEWSLETTER → Archive  
   - SPAM → Archive  
6. Log results  

---


## 🛠 Tools Used

- n8n (workflow automation)  
- Gmail API  
- AI model (classification + reply)  
- Google Sheets  

---

## 📷 Workflow Screenshot

screenshots/workflow.png

---

## 📊 System Diagram

diagrams/system-diagram.png

---

## 📊 Logging Output

All processed emails are saved in Google Sheets:

- timestamp  
- from  
- subject  
- category  
- action  

---


## ✅ Test Results

All scenarios were tested:

- URGENT → draft created ✅  
- IMPORTANT → stays in inbox ✅  
- NEWSLETTER → archived ✅  
- SPAM → archived ✅  

---

## ⚠️ Important Note

The system does NOT send emails automatically.

All replies for urgent emails are saved as drafts for manual review.

---


## 🚀 How to Run

1. Import workflow.json into n8n  
2. Connect Gmail & Google Sheets  
3. Execute workflow  

---

## 👩‍💻 Author

Negma Abdelrahman