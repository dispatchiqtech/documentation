
---

## 3. `docs/architecture.md` (System Architecture)

```markdown
# 🏗 System Architecture

## High-Level Diagram
[Insert diagram here: React frontend ↔ Python FastAPI backend ↔ Supabase (Postgres) ↔ GCP services]

## Components
- **Frontend**: React + Tailwind (PWA)
- **Backend**: FastAPI (Python)
- **Database**: Supabase (Postgres + Auth)
- **Queue/Events**: GCP Pub/Sub
- **Storage**: GCP Cloud Storage
- **Notifications**: Twilio (SMS), SendGrid (Email), Firebase (Push)
- **Payments**: Stripe Connect

## Data Flow
1. Property Manager submits service request.
2. Backend stores job in Supabase.
3. AI Matching Engine scores subcontractors.
4. Notifications dispatched via GCP Pub/Sub workers.
5. Job lifecycle tracked until completion.
6. Invoice generated & Stripe payout triggered.

---
