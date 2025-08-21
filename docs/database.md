# 🗄 Database Schema



## Key Tables
### Users
- id (UUID, PK)
- role (admin, subcontractor, manager)
- name, email, phone
- created_at, updated_at

### Jobs
- id (UUID, PK)
- property_manager_id (FK → users.id)
- subcontractor_id (FK → users.id, nullable)
- status (pending, assigned, en_route, in_progress, completed, closed)
- location (PostGIS point)
- service_type, notes
- created_at, updated_at

### Payments
- id (UUID, PK)
- job_id (FK → jobs.id)
- amount
- stripe_payment_id
- status (pending, paid)

### Documents
- id (UUID, PK)
- subcontractor_id (FK → users.id)
- type (insurance, w9, license)
- url (Cloud Storage path)

---
