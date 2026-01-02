# 🔥 API Testing — 25 Days Real-World Challenge

> **Status codes don’t break systems.  
Assumptions do.**

This repository documents a **25-day hands-on API Testing challenge** focused on how APIs **actually behave in production**, not how they look in tutorials.

If you think `200 OK` means success — this repo will fix that.

---

## 💥 Why This Challenge Exists

Most API testing stops at:

Send request → Check status → Done

Real systems don’t fail that way.

This challenge trains you to:
- Test **what happens after the response**
- Catch **silent async failures**
- Validate **business outcomes**, not messages
- Think like a tester who understands backend systems

---

## 🧠 What You’ll Learn (High-Impact Only)

- How APIs work internally  
  *(Client → API → Service → DB → Queue → Worker)*
- Why async APIs return success before work is done
- How retries cause **duplicate payments**
- Why idempotency is a production lifesaver
- Where to look when users complain *minutes later*
- How to test APIs like a **system**, not an endpoint

---

## ⚔️ The 25-Day Challenge (Big Picture)

### Phase 1 — Foundations That Actually Matter
- How APIs **really** work
- Sync vs Async (no textbook nonsense)
- HTTP beyond status codes
- REST as **state**, not URLs

### Phase 2 — Data, Queues & Failure Reality
- Database persistence & rollbacks
- Message queues & eventual consistency
- Async API testing strategies
- Error handling & negative testing

### Phase 3 — Postman With Intent
- Assertions that catch real bugs
- Polling & async validation
- Pre-request & post-response scripts
- Testing retries and failures

### Phase 4 — Contracts, Security & Observability
- Swagger as a testing contract
- Contract vs reality
- API versioning & backward compatibility
- Auth, rate limiting & abuse cases
- Logs, correlation IDs & tracing

### Phase 5 — REST Assured (Automation With Brain)
- Automation that validates **behavior**
- Async testing with polling (Awaitility)
- DB validation
- Failure simulation
- Final API testing framework project

---

## 🧪 What This Repo Contains

- 📘 Day-wise learning notes  
- 💥 Real production failure scenarios  
- 📮 Postman collections  
- 📄 Swagger findings  
- 🤖 REST Assured automation  
- 🧩 API flow diagrams  
- 🧪 Test cases & validation strategies  

---

## 🛑 What This Repo Is NOT

- ❌ A basic REST tutorial  
- ❌ Tool-only automation snippets  
- ❌ Happy-path testing notes  

This repo focuses on **how systems fail and how testers catch it**.

---

## 🔑 Core API Testing Principles

- HTTP success ≠ business success  
- Async APIs require **waiting and verification**  
- Database is the **source of truth**  
- Logs explain *why*, DB shows *what*  
- Idempotency prevents duplicate disasters  
- Test outcomes, not just responses  

---

## 📂 Repository Structure

```text
API-Testing/
├── day-wise-notes/
├── postman/
├── async-testing/
├── swagger/
├── rest-assured/
├── diagrams/
├── test-cases/
└── README.md
