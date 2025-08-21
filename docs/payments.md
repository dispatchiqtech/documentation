# 💵 Payments & Invoicing

## Flow
1. Job completed.
2. Invoice generated (Stripe or QuickBooks).
3. Property Manager pays invoice.
4. Funds split via Stripe Connect (platform fee + subcontractor payout).
5. Payment status updated in DB.

## Stripe Setup
- Connected Accounts for subcontractors.
- Webhooks: `payment_intent.succeeded`, `payout.paid`.

## Invoice Format
- Job ID
- Property Manager details
- Subcontractor details
- Service description
- Amount, taxes, fees

---
