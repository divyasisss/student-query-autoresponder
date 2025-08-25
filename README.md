# 📧 Automated Student Query Responder (n8n Workflow)

This repository contains an **n8n workflow** that automates student query responses via Google Forms, Google Sheets, and Gmail.

## 🚀 Workflow Overview
1. **Google Form** – Students submit their queries.
2. **Google Sheets Trigger** – Captures new responses automatically.
3. **(Optional) Get Row(s) Node** – Fetches additional sheet data.
4. **Merge Node** – Combines query data with guidelines/responses.
5. **Function (Code) Node** – Categorizes query, generates structured response, ensures email validity.
6. **Gmail Node** – Sends the auto-generated reply email to the student.

## 🛠️ Features
- Prevents duplicate email sends.
- Maps issues (termination, submission, technical, etc.) to predefined responses.
- Sends **structured HTML emails** with candidate details.
- Supports future extensibility for new query types.

## 📂 Repository Structure
```
student-query-autoresponder/
│
├── workflows/
│   └── workflowsstudent-query-autoresponder.json
│
├── README.md
└── .gitignore
```

## ⚡ How to Use
1. Clone this repo:
   ```bash
   git clone https://github.com/YOUR_USERNAME/student-query-autoresponder.git
   ```
2. Open **n8n**.
3. Go to **Import workflow** → upload `workflows/workflowsstudent-query-autoresponder.json`.
4. Set up credentials:
   - Google Sheets
   - Gmail
5. Activate the workflow.

---
