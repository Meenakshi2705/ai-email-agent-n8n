# 🤖 AI Email Agent using n8n

An AI-powered email automation built with **n8n**, **Google Gemini**, and **Gmail** that automatically classifies incoming emails, applies labels, and drafts intelligent responses.

---

## 🚀 Features

- 📩 Automatically triggers on new Gmail messages  
- 🧠 Classifies emails using AI into:
  - Consultation Requests
  - Billing
  - Customer Support
  - Education
- 🏷️ Applies Gmail labels based on classification  
- ✍️ Generates AI-based email replies using Google Gemini  
- 📨 Saves responses as **Gmail drafts** (human-in-the-loop safe)  
- ⚡ Fully automated using n8n workflow  

---
![WhatsApp Image 2025-12-19 at 22 06 49_4cd9397d](https://github.com/user-attachments/assets/c19263af-ed79-464a-b786-1b160a67735b)


## 🧩 Workflow Overview

1. **Gmail Trigger**
   - Listens for new unread emails

2. **AI Text Classification**
   - Uses Google Gemini to classify email content

3. **Category-based Labeling**
   - Automatically assigns Gmail labels:
     - Consultation Request
     - Billing
     - Customer Support
     - Education

4. **AI Response Generation**
   - Generates a contextual reply based on email content

5. **Draft Creation**
   - Saves the AI-generated reply as a Gmail draft in the same thread

---

## 🛠️ Tech Stack

- **n8n** – Workflow automation  
- **Google Gemini (PaLM API)** – AI classification & response generation  
- **Gmail API** – Email trigger, labeling, and draft creation  
- **LangChain (n8n nodes)** – AI orchestration  

---

## ⚙️ Setup Instructions
**Install and run n8n**
- Import email-agent.json into n8n

**Configure credentials:**
-Gmail OAuth
-Google Gemini (PaLM API key)

**Create Gmail labels:**
-Consultation Request
-Billing
-Customer Support
-Education

**Update label IDs in Gmail nodes**
**Activate the workflow**

---

## 📂 Repository Structure

```text
.
├── email-agent.json        # n8n workflow export
├── README.md               # Project documentation
└── screenshots/
    └── workflow.png        # n8n workflow screenshot
