# API Testing Repo – Day 1

## Overview
This repo contains notes, test case templates, and documentation for understanding real API testing principles.  
Focus: Async processing, downstream verification, and system-thinking mindset.

---

## Day 1 – Real API Tester Mindset

### Key Takeaways:
1. **200 OK ≠ Business Success**
   - HTTP success only indicates the request was accepted, not completed.
2. **Async vs Sync APIs**
   - Async APIs return before processing completes.
   - Testing must include DB, queues, logs, and downstream effects.
3. **System Thinking**
   - Consider: downstream systems, message queues, workers, and user impact.
4. **Silent Failures**
   - Failures can happen without any client-visible error.
   - Always check persistence, retries, and idempotency.

---

## Where to Check Failures
- **Database** – source of truth for persistence
- **Logs** – trace workflow, retries, exceptions
- **Queues / Workers** – confirm async processing
- **External Services** – payment, inventory, notifications

---

## Typical Async Failure Diagnosis
Example workflow:
1. API returns 200 → check DB
2. DB record exists → check queue / worker logs
3. Check downstream systems → inventory, payment
4. Confirm no duplicates and user experience is correct

---

## Notes & Reference
- Status code ≠ business success
- Poll async APIs until terminal state
- Validate compensation flows (refunds, retries)
- Trace errors from the system root, not just response

---

## Next Steps
- Day 2: Hands-on Postman testing with async APIs
- Start building test cases, logging results, and documenting in `test-cases/`
