# 📧 Smart Email Automation

An AI-powered email automation workflow built using **n8n**, **Gmail API**, **OpenRouter AI**, and **Airtable** to intelligently manage incoming emails. The workflow automatically classifies emails, generates summaries, detects priorities, applies Gmail labels, stores important information in Airtable, and drafts replies for internship-related emails.

---

## 🚀 Features

- 📬 Automatically monitors new Gmail emails
- 🤖 AI-powered email classification
- 📝 Generates concise email summaries
- ⭐ Assigns High, Medium, or Low priority
- 🏷️ Automatically adds Gmail labels
- 📂 Categorizes emails into:
  - Internship
  - Personal
  - Promotional
  - Payments
  - Updates & Notifications
  - Misleading
- 📊 Saves processed emails to Airtable
- ✍️ Generates AI-powered draft replies for internship emails
- 🗑️ Automatically moves misleading emails to Trash
- ✅ Marks processed emails as read

---

# 🏗️ Workflow Overview

```text
New Email Received
        │
        ▼
 Gmail Trigger
        │
        ▼
 AI Email Classification
        │
 ┌──────┼────────────────────────────────────────────┐
 ▼      ▼         ▼          ▼         ▼            ▼
Personal Internship Promotional Payments Misleading Updates
 │         │          │         │         │          │
 ▼         ▼          ▼         ▼         ▼          ▼
Summary  Draft     Add Label  Add Label  Trash   Add Label
Priority Reply
Category
 │
 ▼
Airtable Database
 │
 ▼
Mark Email as Read
```

---

# ⚙️ Tech Stack

| Technology | Purpose |
|------------|---------|
| n8n | Workflow Automation |
| Gmail API | Email Integration |
| OpenRouter AI | Email Classification & Summarization |
| Airtable | Email Storage |
| JSON Output Parser | Structured AI Output |

---

# 📂 Repository Structure

```
Smart-Email-Automation/
│
├── README.md
├── Email-Categoriser.json
├── assets/
│   ├── workflow.png
│   ├── architecture.png
│   └── demo.gif
```

---

# 📋 Email Categories

The AI classifies every incoming email into one of the following categories:

- 👤 Personal
- 💼 Internship
- 📢 Promotional
- 💳 Payments
- 🔔 Updates & Notifications
- ⚠️ Misleading

---

# 🧠 AI Processing

For every incoming email, the workflow performs:

- Email Classification
- AI-generated Summary
- Priority Detection
- Category Detection
- Gmail Label Assignment
- Airtable Record Creation
- AI Draft Reply (Internship Emails)
- Automatic Cleanup for Misleading Emails

---

# 📷 Workflow

> Replace the image below with your own workflow screenshot.

![Workflow](assets/workflow.png)

---

# 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/anishkumar-1212/Smart-Email-Automation.git
```

### 2. Import the Workflow

Open your n8n instance and import:

```
Email-Categoriser.json
```

### 3. Configure Credentials

Before running the workflow, configure your own credentials for:

- Gmail OAuth2
- OpenRouter API
- Airtable Personal Access Token

### 4. Activate the Workflow

Enable the Gmail Trigger node and activate the workflow.

---

# 🎯 Use Cases

- AI-powered inbox management
- Internship application tracking
- Personal email organization
- Automatic email prioritization
- Email summarization
- Productivity automation

---

# 🔒 Security

This repository does **not** include:

- Gmail credentials
- OAuth secrets
- OpenRouter API keys
- Airtable access tokens

Please configure your own credentials before using the workflow.

---

# 🔮 Future Improvements

- Microsoft Outlook support
- Slack notifications
- Telegram integration
- Discord integration
- Calendar event creation
- Attachment analysis
- Sentiment analysis
- Analytics dashboard
- Multi-user support

---

# 🤝 Contributing

Contributions, suggestions, and improvements are welcome.

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Open a Pull Request

---

# 👨‍💻 Author

**Anish Patel**

- GitHub: https://github.com/anishkumar-1212
- LinkedIn: https://www.linkedin.com/in/anish-kumar-2822691ba

---

## ⭐ If you found this project useful, consider giving it a star!
