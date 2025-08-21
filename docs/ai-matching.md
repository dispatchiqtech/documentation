# 🤖 AI Matching Engine

## Inputs
- Availability
- Distance (Google Maps API)
- Tier level
- Profitability (rate – cost)
- Acceptance history

## Algorithm
```python
score = (
    (profit_weight * profit) +
    (distance_weight * distance_score) +
    (tier_weight * tier_level) +
    (acceptance_weight * acceptance_rate)
)

Output

Ranked subcontractors (top 3).

Auto-dispatch if enabled.

Fallback to next subcontractor if declined.

---

## 7. `docs/job-lifecycle.md` (Job Lifecycle)

```markdown
# 🔄 Job Lifecycle

## Status Flow


Pending → Assigned → En Route → In Progress → Completed → Closed

- **Pending**: New request, waiting for match.
- **Assigned**: Subcontractor selected.
- **En Route**: Subcontractor on way.
- **In Progress**: Work started.
- **Completed**: Work finished, awaiting proof.
- **Closed**: Client approved, invoiced, paid.

## Proof of Completion
- Required: Photos, notes.
- Stored in GCP Storage.

---
