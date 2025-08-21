# DispatchIQ – AI Dispatch & Subcontractor Management Platform

## 🚀 Overview
DispatchIQ is a SaaS platform that automates intelligent job dispatching for property management companies and subcontractors.  
Tech stack: **Python (FastAPI), React.js, Supabase, Tailwind, GCP**.

Core modules:
- Service request intake
- AI subcontractor matching
- Job dispatch & lifecycle tracking
- Invoicing & payouts

---

## 👥 Roles
- **Admin/Dispatcher**
- **Subcontractor**
- **Property Manager**
- **API Client (Post-MVP)**

---

## 📖 Docs Index
- [Setup Guide](docs/setup.md)
- [System Architecture](docs/architecture.md)
- [Database Schema](docs/database.md)
- [API Reference](docs/api.md)
- [AI Matching Engine](docs/ai-matching.md)
- [Job Lifecycle](docs/job-lifecycle.md)
- [Payments & Invoicing](docs/payments.md)
- [Contribution Guide](docs/contributing.md)

---

## 🛠 Quick Start
```bash
# clone repo
git clone https://github.com/org/dispatchiq.git
cd dispatchiq

# start backend
cd backend && pip install -r requirements.txt && uvicorn app.main:app --reload

# start frontend
cd frontend && npm install && npm run dev
