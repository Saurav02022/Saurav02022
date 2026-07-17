# Saurav Kumar

**I build software that keeps working when the network doesn't.**

Full-stack + LLM engineer, 3+ years in production. Based in Mumbai, open to relocating. I own the whole path — API to deploy — and design for the parts that actually break: the connection that drops, the model that answers off-schema, the vendor API that fires the same webhook twice. The unglamorous work — retry logic, idempotent writes, the reconnect path — is usually where a product is won or lost.

## What I focus on

- **Owning the whole path** — API, database schema, and deploy, not just the UI.
- **Reliability under bad conditions** — idempotent writes, offline-first sync, retries that never double-write.
- **Schema-locked LLM features** — model output pinned to a schema with deterministic fallbacks, so a flaky model can't corrupt the app.
- **Tests that gate deploys** — E2E and unit suites wired into CI, so a red build doesn't ship.

## Experience

**Shikha Learning Labs** — Software Engineer · EdTech · Nov 2024–present

- 4 production apps (web + Android) across **117 schools**, holding **96%+ crash-free** on a shared Next.js API layer and a PostgreSQL schema I designed.
- Cut a teacher's grading pass from **40 minutes to 5–10** with an async Redis queue and FastAPI workers on Gemini — now **400+ evaluations a week** for **200+ teachers**.
- **98% API success over 5,000+ submissions** with idempotent retries against a fixed schema; stopped data loss at **50+ low-network schools** with an offline-first IndexedDB queue.

**Nuveb** — Full-Stack Developer · Creator OTT platform · May 2023–Sep 2024

- Built the creator portal's video, scheduling, and payment modules as it grew from **0 to 10,000+ creators**.
- Cut page load **8.5s → 2.5s** for **50,000+ monthly users** (moved over-fetched catalogue pages from SSR to SSG); dropped image API latency **3.2s → 1.9s** with server-side Sharp.

*Company source is private — the projects below are where you can read my code.*

## Selected projects

- **[AI Résumé Builder](https://github.com/Saurav02022/resume-builder)** — tailors a résumé to a job with Gemini pinned to a Pydantic schema at temperature 0, a side-by-side diff you approve before export, and LaTeX/PDF output. 31 Playwright tests gate the deploy. `Next.js · FastAPI · Gemini` · [live](https://resume-builder-saurav02022.vercel.app)
- **[RTO Shield](https://github.com/Saurav02022/rto-shield)** — a voice-AI console that confirms risky cash-on-delivery orders before dispatch. At-least-once webhooks made exactly-once over a ports/adapters store (in-memory for tests, Firestore in prod). 19 pytest + 14 Vitest. `FastAPI · Next.js · Bolna`
- **[Claims Adjudication Engine](https://github.com/Saurav02022/claims-processing-system)** — health-insurance claims through a pure Decimal engine and a single atomic Postgres function, with append-only history. 74 tests — more test code than app code. `FastAPI · PostgreSQL · Supabase`
- **[Intervue](https://github.com/Saurav02022/ai-interview)** — a mock-interview marketplace: book with credits, transcribed video call, AI feedback after. Idempotent payout keyed on the booking, Clerk JWTs verified via JWKS, keyless deploys gated on a container smoke test. `Next.js · FastAPI · Stream · Gemini`

Full write-ups, plus two more builds → **[portfolio](https://saurav02022-portfolio.vercel.app)**

## Stack

- **Languages** — TypeScript · Python · JavaScript · SQL
- **Frontend** — Next.js · React · React Native
- **Backend** — FastAPI · Node.js
- **Data** — PostgreSQL · Redis · Firestore · IndexedDB
- **LLM** — Google Gemini (schema-locked)
- **Cloud & CI** — Docker · GCP Cloud Run · Vercel · GitHub Actions
- **Testing & monitoring** — Playwright · pytest · Sentry

## Links

[Portfolio](https://saurav02022-portfolio.vercel.app) · [LinkedIn](https://linkedin.com/in/saurav02022) · [LeetCode](https://leetcode.com/u/Saurav02022) · [Email](mailto:sk729584@gmail.com)
