<div align="center">

# Saurav Kumar

**I build software that keeps working when the network doesn't.**

Full-stack + LLM engineer · 3+ years in production · Mumbai, open to relocating

[![Portfolio](https://img.shields.io/badge/Portfolio-0A6B57?style=flat-square&logo=vercel&logoColor=white)](https://saurav02022-portfolio.vercel.app)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/saurav02022)
[![LeetCode](https://img.shields.io/badge/LeetCode-FFA116?style=flat-square&logo=leetcode&logoColor=white)](https://leetcode.com/u/Saurav02022)
[![Email](https://img.shields.io/badge/Email-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:sk729584@gmail.com)

</div>

---

I own the whole path — API to deploy — and design for the parts that actually break: the connection that drops, the model that answers off-schema, the vendor API that fires the same webhook twice. The unglamorous work — retry logic, idempotent writes, the reconnect path — is usually where a product is won or lost.

## ⚡ What I focus on

- **Owning the whole path** — API, database schema, and deploy, not just the UI.
- **Reliability under bad conditions** — idempotent writes, offline-first sync, retries that never double-write.
- **Schema-locked LLM features** — model output pinned to a schema with deterministic fallbacks, so a flaky model can't corrupt the app.
- **Tests that gate deploys** — E2E and unit suites wired into CI, so a red build doesn't ship.

## 💼 Experience

**Shikha Learning Labs** — Software Engineer · EdTech · Nov 2024–present

- 4 production apps (web + Android) across **117 schools**, holding **96%+ crash-free** on a shared Next.js API layer and a PostgreSQL schema I designed.
- Cut a teacher's grading pass from **40 minutes to 5–10** with an async Redis queue and FastAPI workers on Gemini — now **400+ evaluations a week** for **200+ teachers**.
- **98% API success over 5,000+ submissions** with idempotent retries against a fixed schema; stopped data loss at **50+ low-network schools** with an offline-first IndexedDB queue.

**Nuveb** — Full-Stack Developer · Creator OTT platform · May 2023–Sep 2024

- Built the creator portal's video, scheduling, and payment modules as it grew from **0 to 10,000+ creators**.
- Cut page load **8.5s → 2.5s** for **50,000+ monthly users** (over-fetched catalogue pages moved SSR → SSG); dropped image API latency **3.2s → 1.9s** with server-side Sharp.

_Company source is private — the projects below are where you can read my code._

## 📦 Selected projects

### [AI Résumé Builder](https://github.com/Saurav02022/resume-builder)
[![live](https://img.shields.io/badge/live-2E9E62?style=flat-square&logo=vercel&logoColor=white)](https://resume-builder-saurav02022.vercel.app) ![tests](https://img.shields.io/badge/tests-31-0A6B57?style=flat-square)

Tailors a résumé to a job — Gemini pinned to a Pydantic schema at temperature 0, a diff you approve before anything exports, and LaTeX/PDF out. The Playwright suite gates the Vercel deploy.

`Next.js` · `FastAPI` · `Gemini` · `Playwright`

### [RTO Shield](https://github.com/Saurav02022/rto-shield)
![tests](https://img.shields.io/badge/tests-33-0A6B57?style=flat-square)

A voice-AI console that confirms risky cash-on-delivery orders before they ship. Bolna's webhooks fire more than once; a ports/adapters store (in-memory for tests, Firestore in prod) and one call-ID-keyed handler make at-least-once delivery land exactly once.

`FastAPI` · `Next.js` · `Bolna` · `Firestore`

### [Claims Adjudication Engine](https://github.com/Saurav02022/claims-processing-system)
![tests](https://img.shields.io/badge/tests-74-0A6B57?style=flat-square)

Adjudicates health-insurance claims through a pure Decimal engine and a single atomic Postgres function, with append-only history. More test code than application code.

`FastAPI` · `PostgreSQL` · `Supabase` · `pytest`

### [Intervue — Mock-Interview Marketplace](https://github.com/Saurav02022/ai-interview)
![keyless CD](https://img.shields.io/badge/keyless_CD-4285F4?style=flat-square&logo=googlecloud&logoColor=white)

Book with credits, meet on a transcribed video call, get AI feedback after. The post-call payout is an idempotent upsert keyed on the booking, so a retried webhook never pays twice; Clerk JWTs are verified via JWKS, and deploys are keyless and gated on a container smoke test.

`Next.js` · `FastAPI` · `Stream` · `Clerk` · `Gemini`

### [LinkedIn Hashtag Refresh Engine](https://github.com/Saurav02022/linkedin-hashtag-refresh-engine-app)

Drafts three hashtag sets for a LinkedIn post and posts your pick as a comment. Hand-rolled OIDC refresh, every request body validated behind one typed error envelope, and Sentry wired across client, server, and edge.

`Next.js` · `NextAuth` · `Gemini` · `Sentry`

### [Financial Literacy Assistant](https://github.com/Saurav02022/financial-literacy-assistant)
![tests](https://img.shields.io/badge/tests-10-0A6B57?style=flat-square) ![hackathon](https://img.shields.io/badge/hackathon-6C6558?style=flat-square)

Budgeting, saving, and investing coaching where the math is deterministic TypeScript and Gemini only writes the words on top — with a fixed fallback when the model is down. Built in a 3-hour hackathon.

`Next.js` · `Supabase` · `Gemini` · `Vitest`

## 🧰 Tech stack

**Languages**
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logoColor=white)

**Frontend**
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![React Native](https://img.shields.io/badge/React_Native-20232A?style=flat-square&logo=react&logoColor=61DAFB)

**Backend**
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-5FA04E?style=flat-square&logo=nodedotjs&logoColor=white)

**Data**
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-FF4438?style=flat-square&logo=redis&logoColor=white)
![Firestore](https://img.shields.io/badge/Firestore-DD2C00?style=flat-square&logo=firebase&logoColor=white)
![IndexedDB](https://img.shields.io/badge/IndexedDB-4479A1?style=flat-square)

**LLM**
![Google Gemini](https://img.shields.io/badge/Google_Gemini-8E75B2?style=flat-square&logo=googlegemini&logoColor=white)

**Cloud & CI**
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Google Cloud Run](https://img.shields.io/badge/Cloud_Run-4285F4?style=flat-square&logo=googlecloud&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=flat-square&logo=vercel&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)

**Testing & monitoring**
![Playwright](https://img.shields.io/badge/Playwright-2EAD33?style=flat-square&logo=playwright&logoColor=white)
![pytest](https://img.shields.io/badge/pytest-0A9EDC?style=flat-square&logo=pytest&logoColor=white)
![Sentry](https://img.shields.io/badge/Sentry-362D59?style=flat-square&logo=sentry&logoColor=white)

---

<div align="center">

Open to full-stack / AI engineering roles · will relocate

[**Portfolio**](https://saurav02022-portfolio.vercel.app) · [**LinkedIn**](https://linkedin.com/in/saurav02022) · [**LeetCode**](https://leetcode.com/u/Saurav02022) · [**Email**](mailto:sk729584@gmail.com)

</div>
