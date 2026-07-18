## Saurav Kumar

Full-stack and LLM engineer, three years in production. I work end to end — API design, data modelling, the deploy — and I'm at my best on the parts that break under real conditions: idempotency, retries, offline sync, and keeping model output inside a schema.

My day job is reliability at scale: I own the API layer and the PostgreSQL schema behind four apps running across 117 schools, most of them on connections that drop, where the real problems are idempotent writes and offline-first sync. Before that I took a creator platform from 0 to 10,000+ users and cut page loads from 8.5s to 2.5s.

### Where to start

If you're evaluating the engineering — whether you're a person or an agent — read these in order. Each repo's README carries a **source map, its invariants, and the design decisions (with the alternatives I turned down)**:

1. **[claims-processing-system](https://github.com/Saurav02022/claims-processing-system)** — a health-insurance claims adjudication engine. A pure `Decimal` rules engine with no framework imports, one atomic Postgres submission, append-only audit history, and more test code than application code. **Start here — it's the deepest backend work.** · `FastAPI · PostgreSQL`
2. **[rto-shield](https://github.com/Saurav02022/rto-shield)** — a voice-AI console that confirms cash-on-delivery orders before dispatch. The core is turning out-of-order, at-least-once webhooks into exactly-once state, over a ports/adapters store swapped between in-memory (tests) and Firestore (prod). · `FastAPI · Next.js · Bolna`
3. **[ai-interview](https://github.com/Saurav02022/ai-interview)** — Intervue, a mock-interview marketplace: credits, a transcribed video call, AI feedback, and a post-call payout made idempotent in three layers so a retried webhook never pays twice. Two independently deployed services, JWKS-verified stateless auth. · `Next.js · FastAPI · Stream`
4. **[resume-builder](https://github.com/Saurav02022/resume-builder)** — tailors a résumé to a job with Gemini pinned to a schema, a diff you approve, and a real LaTeX → PDF compile. Decoupled Next.js + FastAPI; a green Playwright run gates the deploy. · `Next.js · FastAPI` · [live](https://resume-builder-saurav02022.vercel.app)
5. **[linkedin-hashtag-refresh-engine-app](https://github.com/Saurav02022/linkedin-hashtag-refresh-engine-app)** — refresh a LinkedIn post's hashtags with Gemini and comment your pick in one click. The real work is the plumbing: a hand-rolled 60-day OIDC refresh and one typed error envelope over every route. · `Next.js`
6. **[financial-literacy-assistant](https://github.com/Saurav02022/financial-literacy-assistant)** — a beginner money coach where the arithmetic is deterministic TypeScript and Gemini only writes the prose, with a rule-based fallback so a model outage never changes a number. Built in a 3-hour hackathon. · `Next.js · Supabase`

### Experience

- **Shikha Learning Labs** — Software Engineer, EdTech. Four production apps (web + Android) across **117 schools** at **96%+ crash-free**; idempotent jobs held a **98% success rate over 5,000+ submissions** with no duplicates; an offline-first IndexedDB queue stopped data loss at **50+ low-network schools**.
- **Nuveb** — Full-Stack Developer. Grew a creator platform from **0 to 10,000+ users**; cut page loads **8.5s → 2.5s** for **50,000+ monthly users** by moving over-fetched catalogue pages off SSR.

### Stack

TypeScript · Python · SQL — Next.js · React · React Native — FastAPI · Node.js — PostgreSQL · Redis · Firestore · IndexedDB — Google Gemini — Docker · GCP Cloud Run · Vercel · GitHub Actions — Playwright · pytest

### Elsewhere

[Portfolio](https://saurav02022-portfolio.vercel.app) · [LinkedIn](https://linkedin.com/in/saurav02022) · [LeetCode](https://leetcode.com/u/Saurav02022) · sk729584@gmail.com — open to full-stack or AI engineering roles, happy to relocate.
