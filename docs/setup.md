
---

## 2. `docs/setup.md` (Environment Setup)

```markdown
# 🛠 Setup Guide

## Prerequisites
- Python 3.11+
- Node.js 18+
- Docker & Docker Compose
- GCP SDK
- Supabase CLI

## Backend Setup
```bash
cd backend
pip install -r requirements.txt
cp .env.example .env
uvicorn app.main:app --reload

Frontend Setup

cd frontend
npm install
npm run dev


Supabase Setup
Create project in Supabase Dashboard
Run migrations: supabase db push.

GCP Setup
Enable Cloud Run, Cloud SQL, Pub/Sub.
Configure secrets in Secret Manager.

