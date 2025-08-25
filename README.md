# student-query-autoresponder
Student Query Autoresponder (n8n Workflow) An automation workflow built with n8n to handle student queries from Google Forms → Google Sheets → Gmail.  Fetches new queries only  Maps issues to exam guidelines  Generates structured replies  Sends automated responses via Gmail.
# Student Query Auto-Responder (n8n Workflow)

This project automates handling of student queries using **n8n**.  
It fetches queries submitted via Google Forms, processes them against predefined exam guidelines, and sends structured email responses automatically.

## 🔄 Workflow Steps
1. **Google Form** → Student submits their query.  
2. **Google Sheet (Get Row(s))** → Fetches query details.  
3. **Merge Node** → Combines query with response guidelines.  
4. **Function Node** → Classifies query type, applies rules, generates reply.  
5. **Gmail Node** → Sends structured auto-response to the student.  

## 🚀 Features
- Prevents duplicate emails (only one mail per student).  
- Categorizes queries (Termination, Technical, Submission, Code/Test, Marks, Interview, General).  
- Uses exam guidelines for accurate, rule-based replies.  
- Sends clean, structured email templates.  

## 📂 Files
- `workflowsstudent-query-autoresponder.json` → The n8n workflow file (can be imported into your n8n instance).  

## 🛠️ Setup
1. Clone this repo:
   ```bash
   git clone https://github.com/divyasisss/student-query-autoresponder.git
