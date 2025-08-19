# 🤖 HR_Expert Agent – Recruitment AI  

An **AI-powered Recruitment Assistant** that automates the hiring pipeline – from **resume screening** to **interview scheduling** – helping recruiters save time, reduce bias, and hire the right talent faster.  

---

## ✨ Key Features  

- **📂 Resume Screening & Parsing**  
  - Extracts skills, experience, and education from resumes (PDF/DOCX).  
  - Ranks candidates based on job description alignment.  
  - Detects missing/extra skills using semantic matching.  

- **🎯 Candidate Matching**  
  - AI-driven scoring of candidates vs. job postings.  
  - Supports multiple roles and skill levels.  
  - Highlights top candidates instantly.  

- **📅 Interview Scheduling**  
  - Integrates with Google Calendar / Outlook.  
  - Automates candidate communication (email/WhatsApp/Slack).  
  - Tracks interview feedback and panel availability.  

- **📊 Recruitment Analytics**  
  - Time-to-hire & candidate pipeline metrics.  
  - Diversity and bias monitoring (optional).  
  - Predictive analytics for candidate success.  

- **🗣️ Conversational Recruitment**  
  - Answers candidate FAQs (role, salary range, process).  
  - Can be embedded in career sites as a chatbot.  
  - Supports multilingual candidate interactions.  

---

## 🏗️ Architecture  

```
+-------------------+        +---------------------+        +-------------------+
|   Candidate UI    | <----> |   HR_Expert Core    | <----> |  Data Sources     |
| (Web, Chatbot)    |        | (AI + Recruit Logic)|        | (Resumes, JD DB)  |
+-------------------+        +---------------------+        +-------------------+
                                    |
                                    v
                            +-------------------+
                            |  Scheduling &     |
                            |  Analytics Engine |
                            +-------------------+
```

- **Frontend**: Career page chatbot / recruiter dashboard  
- **Core Engine**: Resume parser + Candidate-JD matcher (LLM + embeddings)  
- **Integrations**: ATS, Calendars, Email APIs  

---

## 🚀 Getting Started  

### 1️⃣ Clone the repository  
```bash
git clone https://github.com/your-username/HR_Expert.git
cd HR_Expert
```

### 2️⃣ Install dependencies  
```bash
pip install -r requirements.txt
```

### 3️⃣ Configure environment variables  
Create a `.env` file with the following keys:  
```
OPENAI_API_KEY=your_api_key
DB_URL=your_database_url
CALENDAR_API_KEY=your_calendar_api
EMAIL_API_KEY=your_email_api
```

### 4️⃣ Run the Recruitment Agent  
```bash
python app.py
```

Access dashboard at: `http://localhost:8000`  

---

## 🛠️ Tech Stack  

- **Language**: Python (FastAPI / Flask)  
- **AI Models**: GPT-4 / embeddings for resume-JD matching  
- **Database**: PostgreSQL / Supabase / MongoDB  
- **Integrations**: Google Calendar API, Outlook API, Email APIs (SendGrid/Twilio)  
- **Deployment**: Docker, Render, AWS/GCP/Azure  

---

## 📌 Roadmap  

- [ ] Advanced candidate ranking dashboard  
- [ ] Multi-job posting support with bulk resume uploads  
- [ ] Automated recruiter summaries for each candidate  
- [ ] Candidate chatbot for pre-screening questions  
- [ ] Predictive analytics on candidate success  

---

## 🤝 Contributing  

We welcome contributions! Please fork the repo and submit a pull request, or open an issue to suggest features.  

---

## 📄 License  

Distributed under the MIT License. See `LICENSE` for details.  

---

## 🌐 Connect  

👤 **Maintainer**: Maheen Meshram
📧 Email: maheenmeshram.2115@gmail.com  
💼 LinkedIn: nkedin.com/in/maheen-meshram-965066284/  
 

---

⚡ With **HR_Expert Recruitment Agent**, recruiters can focus on people, not paperwork.  
