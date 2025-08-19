# 🤖 HR_Expert Agent – Recruitment AI (n8n)  

An **AI-powered Recruitment Assistant built on n8n** that automates the hiring pipeline – from **resume screening** to **interview scheduling** – helping recruiters save time, reduce bias, and hire the right talent faster.  

---

## ✨ Key Features  

- **📂 Resume Screening & Parsing**  
  - Extracts candidate skills, education, and experience from resumes.  
  - Uses LLMs + embeddings to match resumes with job descriptions.  
  - Flags top candidates automatically.  

- **🎯 Candidate Matching**  
  - AI-driven ranking of candidates for specific roles.  
  - Supports bulk resume uploads.  
  - Semantic matching beyond keyword search.  

- **📅 Interview Scheduling**  
  - Automated calendar invites (Google Calendar, Outlook).  
  - Sends candidate emails via Gmail/SendGrid/Twilio.  
  - Tracks recruiter & panel availability.  

- **📊 Recruitment Analytics**  
  - Pipeline visualization inside n8n.  
  - Metrics: time-to-hire, candidate drop-off, recruiter productivity.  
  - Custom dashboards via Google Sheets / Supabase.  

- **🗣️ Conversational Recruitment**  
  - Candidate FAQ bot (WhatsApp, Slack, Webchat).  
  - Pre-screening via conversational flows.  
  - Multilingual interactions.  

---

## 🏗️ Architecture  

```
+-------------------+        +-------------------+        +-------------------+
|   Candidate Input | <----> |   n8n Workflows   | <----> |  HR Data Sources  |
| (Resume, Chatbot) |        | (AI + Automation) |        | (ATS, Sheets, DB) |
+-------------------+        +-------------------+        +-------------------+
                                    |
                                    v
                            +-------------------+
                            |  Scheduling &     |
                            |  Analytics Engine |
                            +-------------------+
```

- **Core Engine**: n8n workflows + AI nodes (LLM, embeddings).  
- **Integrations**: Gmail, Google Drive, Supabase, Slack, Twilio, ATS APIs.  
- **Storage**: Supabase / PostgreSQL / Google Sheets.  

---

## 🚀 Getting Started  

### 1️⃣ Clone this repository  
```bash
git clone https://github.com/your-username/HR_Expert.git
cd HR_Expert
```

### 2️⃣ Install & Run n8n  
You can run n8n via npm, Docker, or n8n cloud.  
```bash
npm install n8n -g
n8n start
```
or with Docker:  
```bash
docker run -it --rm   -p 5678:5678   -v ~/.n8n:/home/node/.n8n   n8nio/n8n
```

### 3️⃣ Import Workflows  
- Go to `http://localhost:5678`  
- Import the workflows from `/workflows/hr_expert_recruitment.json`  
- Configure credentials for:  
  - OpenAI/Gemini (resume parsing & matching)  
  - Gmail/SendGrid (emailing)  
  - Google Calendar (scheduling)  
  - Database (Supabase/Postgres)  

### 4️⃣ Run the Recruitment Agent  
Once activated, the workflows will:  
1. Parse resumes from a folder or email inbox.  
2. Match them with job descriptions.  
3. Schedule interviews automatically.  
4. Send analytics to a Google Sheet / Supabase dashboard.  

---

## 🛠️ Tech Stack  

- **Workflow Engine**: [n8n](https://n8n.io)  
- **AI Models**: GPT-4 / Gemini Pro / Embeddings  
- **Integrations**: Gmail, Google Calendar, Supabase, Slack, Twilio  
- **Deployment**: n8n Cloud / Docker / Self-hosted  

---

## 📌 Roadmap  

- [ ] Bulk candidate ranking dashboard  
- [ ] Recruiter chatbot (Slack integration)  
- [ ] Candidate WhatsApp pre-screening  
- [ ] Predictive analytics (attrition, candidate success)  

---

## 🤝 Contributing  

We welcome contributions! Fork the repo, create your workflow, and submit a PR.  

---

## 📄 License  

Distributed under the MIT License. See `LICENSE` for details.  

---

## 🌐 Connect  

👤 **Maintainer**: [Your Name / Team]  
📧 Email: your@email.com  
💼 LinkedIn: [Your LinkedIn]  
🚀 Demo: [Live Demo Link if available]  

---

⚡ With **HR_Expert Recruitment Agent (n8n)**, recruiters can focus on people, not paperwork.  
