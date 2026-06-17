# 🚀 CourseReach AI

> AI-Powered Lead Discovery, Qualification & Personalized Outreach Platform for Educational Businesses

![Next.js](https://img.shields.io/badge/Next.js-15-black)
![FastAPI](https://img.shields.io/badge/FastAPI-Latest-green)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-Database-blue)
![OpenAI](https://img.shields.io/badge/OpenAI-LLM-orange)
![License](https://img.shields.io/badge/License-MIT-yellow)

---

## 📖 Overview

CourseReach AI is an AI-powered lead discovery and outreach platform designed for educational organizations, training institutes, and EdTech companies.

The platform automates:

- Lead Discovery
- Lead Qualification
- Course Recommendation
- Personalized Outreach Generation
- Campaign Management
- Analytics & Reporting

Using AI agents, the platform analyzes lead profiles, recommends suitable courses, generates personalized outreach messages, and tracks campaign performance.

---

## ✨ Features

### 🔍 Lead Discovery
- Import leads through CSV
- Public business directory integration
- Lead organization and filtering
- Duplicate detection

### 🤖 AI Lead Qualification
- Industry classification
- Role identification
- Lead scoring
- Audience segmentation

### 🎯 Course Recommendation
- Intelligent course matching
- Industry-aware recommendations
- Skill-based targeting

### ✉️ Personalized Outreach
- AI-generated email subjects
- Personalized email content
- Follow-up email generation
- Campaign-specific messaging

### 📊 Analytics Dashboard
- Total Leads
- Qualified Leads
- Open Rate
- Click Rate
- Reply Rate
- Campaign Performance

### 🔐 Security
- JWT Authentication
- Role-Based Access Control
- Password Hashing
- Rate Limiting
- Audit Logging

---

## 🏗️ System Architecture

```text
                ┌─────────────────┐
                │   Frontend UI   │
                │    Next.js      │
                └────────┬────────┘
                         │
                         ▼
                ┌─────────────────┐
                │  FastAPI Backend│
                └────────┬────────┘
                         │

      ┌──────────────────┼──────────────────┐
      ▼                  ▼                  ▼

┌─────────────┐   ┌─────────────┐   ┌─────────────┐
│Qualification│   │Course Match │   │Outreach AI  │
│   Agent     │   │    Agent    │   │    Agent    │
└─────────────┘   └─────────────┘   └─────────────┘

                         │
                         ▼

                ┌─────────────────┐
                │   PostgreSQL    │
                └─────────────────┘

                         │
                         ▼

                ┌─────────────────┐
                │ Email Provider  │
                │ Resend/SendGrid │
                └─────────────────┘
```

---

## 🛠️ Tech Stack

### Frontend
- Next.js 15
- TypeScript
- Tailwind CSS
- Shadcn UI

### Backend
- FastAPI
- SQLAlchemy
- PostgreSQL
- Redis

### AI Layer
- OpenAI API
- Agent-Based Workflow

### Infrastructure
- Docker
- Docker Compose
- Nginx

---

## 📂 Project Structure

```bash
course-reach-ai/

├── frontend/
│   ├── app/
│   ├── components/
│   ├── hooks/
│   ├── lib/
│   └── types/
│
├── backend/
│   ├── api/
│   ├── agents/
│   ├── database/
│   ├── models/
│   ├── schemas/
│   ├── services/
│   ├── workers/
│   └── utils/
│
├── docs/
├── docker/
├── scripts/
│
├── docker-compose.yml
├── .env.example
└── README.md
```

---

## ⚙️ Installation

### Clone Repository

```bash
git clone https://github.com/yourusername/course-reach-ai.git

cd course-reach-ai
```

### Backend Setup

```bash
cd backend

python -m venv venv

# Linux/Mac
source venv/bin/activate

# Windows
venv\Scripts\activate

pip install -r requirements.txt
```

### Frontend Setup

```bash
cd frontend

npm install
```

---

## 🔑 Environment Variables

Create a `.env` file:

```env
DATABASE_URL=postgresql://user:password@localhost/course_reach

OPENAI_API_KEY=your_openai_key

JWT_SECRET=your_secret_key

REDIS_URL=redis://localhost:6379

EMAIL_PROVIDER=resend

RESEND_API_KEY=your_api_key
```

---

## ▶️ Running the Application

### Start Backend

```bash
uvicorn main:app --reload
```

### Start Frontend

```bash
npm run dev
```

### Access Application

| Service | URL |
|----------|----------|
| Frontend | http://localhost:3000 |
| Backend | http://localhost:8000 |
| API Docs | http://localhost:8000/docs |

---

## 🐳 Docker Deployment

Build and start containers:

```bash
docker-compose up --build
```

Run in background:

```bash
docker-compose up -d
```

Stop containers:

```bash
docker-compose down
```

---

## 🤖 AI Workflow

```text
Lead Discovery
      ↓
Lead Qualification
      ↓
Course Recommendation
      ↓
Personalized Email Generation
      ↓
Campaign Management
      ↓
Email Delivery
      ↓
Analytics Tracking
```

---

## 📊 Database Schema

### Users

```sql
id
name
email
password_hash
role
created_at
```

### Leads

```sql
id
name
email
company
industry
designation
website
location
source
relevance_score
recommended_course
created_at
```

### Courses

```sql
id
title
description
category
price
created_at
```

### Campaigns

```sql
id
name
course_id
status
created_at
```

### Outreach Messages

```sql
id
lead_id
campaign_id
subject
message
status
sent_at
```

---

## 📈 Future Enhancements

- CRM Integrations
- WhatsApp Business Integration
- AI Campaign Optimization
- Multi-Tenant SaaS Architecture
- Advanced Lead Scoring
- Automated Reporting
- Team Collaboration
- Workflow Automation

---

## 🎯 Use Cases

### Educational Platforms
Promote certification programs and online courses.

### Training Institutes
Reach professionals interested in upskilling.

### Corporate Learning Providers
Identify organizations seeking employee training programs.

### EdTech Startups
Scale outreach and lead generation efficiently.

---

## 🤝 Contributing

Contributions are welcome!

1. Fork the repository

2. Create a feature branch

```bash
git checkout -b feature-name
```

3. Commit changes

```bash
git commit -m "Add feature"
```

4. Push to GitHub

```bash
git push origin feature-name
```

5. Open a Pull Request

---

## 📜 License

This project is licensed under the MIT License.

---

## 👨‍💻 Author

**Aditya Yadav**

Built with:

- Next.js
- FastAPI
- PostgreSQL
- OpenAI
- Docker
- Agentic AI Workflows

---

⭐ If you found this project useful, consider giving it a star on GitHub.
