🚀 CourseReach AI

«AI-Powered Lead Discovery, Qualification, and Personalized Outreach Platform for Educational Businesses»

"Next.js" (https://img.shields.io/badge/Next.js-15-black)
"FastAPI" (https://img.shields.io/badge/FastAPI-Latest-green)
"PostgreSQL" (https://img.shields.io/badge/PostgreSQL-Database-blue)
"OpenAI" (https://img.shields.io/badge/OpenAI-LLM-orange)
"License" (https://img.shields.io/badge/License-MIT-yellow)

📖 Overview

CourseReach AI is an intelligent lead discovery and outreach platform designed for educational organizations, training institutes, and EdTech companies.

The platform automates the process of:

- Discovering potential leads
- Qualifying prospects using AI
- Recommending relevant courses
- Generating personalized outreach emails
- Managing marketing campaigns
- Tracking engagement analytics

Instead of sending generic marketing messages, CourseReach AI uses AI agents to understand lead profiles and generate personalized communication tailored to each prospect.

---

✨ Key Features

🔍 Lead Discovery

- Public business source integration
- Lead import via CSV
- Company and contact management
- Duplicate lead detection
- Lead filtering and segmentation

🤖 AI Lead Qualification

- Industry identification
- Job role classification
- Relevance scoring
- Prospect segmentation

🎯 Course Recommendation Engine

- Match leads to relevant courses
- Skill-based recommendations
- Industry-aware suggestions

✉️ Personalized Outreach

- AI-generated email subjects
- Personalized email content
- Follow-up sequences
- Campaign-specific messaging

📊 Analytics Dashboard

- Lead statistics
- Open rates
- Click rates
- Reply tracking
- Campaign performance metrics

🔐 Secure & Scalable

- JWT Authentication
- Role-Based Access Control
- Rate Limiting
- Audit Logging
- Docker Deployment

---

🏗️ System Architecture

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
│ Qualification│   │ Course Match│   │ Outreach AI │
│    Agent     │   │    Agent    │   │    Agent    │
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

---

🛠 Tech Stack

Frontend

- Next.js 15
- TypeScript
- Tailwind CSS
- Shadcn UI

Backend

- FastAPI
- SQLAlchemy
- PostgreSQL
- Redis

AI Layer

- OpenAI API
- Agent-Based Workflow

Infrastructure

- Docker
- Docker Compose
- Nginx

---

📂 Project Structure

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
├── docker/
├── docs/
├── scripts/
│
├── docker-compose.yml
├── .env.example
└── README.md

---

⚙️ Installation

Clone Repository

git clone https://github.com/yourusername/course-reach-ai.git

cd course-reach-ai

Backend Setup

cd backend

python -m venv venv

source venv/bin/activate
# Windows
venv\Scripts\activate

pip install -r requirements.txt

Frontend Setup

cd frontend

npm install

---

🔑 Environment Variables

Create a ".env" file:

DATABASE_URL=postgresql://user:password@localhost/course_reach

OPENAI_API_KEY=your_openai_key

JWT_SECRET=your_secret_key

REDIS_URL=redis://localhost:6379

EMAIL_PROVIDER=resend

RESEND_API_KEY=your_api_key

---

▶️ Running the Application

Start Backend

uvicorn main:app --reload

Start Frontend

npm run dev

Access Application

Frontend:
http://localhost:3000

Backend:
http://localhost:8000

Swagger Docs:
http://localhost:8000/docs

---

🐳 Docker Deployment

Build and run:

docker-compose up --build

Run in background:

docker-compose up -d

Stop containers:

docker-compose down

---

📊 Core AI Workflow

Lead Discovery
        │
        ▼
Lead Qualification
        │
        ▼
Course Recommendation
        │
        ▼
Personalized Email Generation
        │
        ▼
Campaign Management
        │
        ▼
Email Delivery
        │
        ▼
Analytics Tracking

---

📈 Future Roadmap

- CRM Integrations
- WhatsApp Business Support
- AI Campaign Optimization
- Multi-Tenant SaaS Architecture
- Advanced Lead Scoring
- Automated Reporting
- Team Collaboration Features
- Workflow Automation

---

🎯 Use Cases

Educational Platforms

Promote certification and professional development programs.

Training Institutes

Reach targeted professionals and students.

Corporate Learning Providers

Identify organizations interested in employee upskilling.

EdTech Startups

Scale lead generation and outreach efficiently.

---

🤝 Contributing

Contributions are welcome.

1. Fork the repository
2. Create a feature branch
3. Commit changes
4. Open a Pull Request

---

📜 License

MIT License

---

👨‍💻 Author

Aditya Yadav

Built as an AI-powered SaaS project combining:

- Large Language Models (LLMs)
- Agentic AI Workflows
- FastAPI
- PostgreSQL
- Next.js
- Marketing Automation
