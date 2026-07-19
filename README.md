## Saurav Kumar

Full-stack and AI engineer, three years in production. I build the whole thing — the API, the database, the deploy — and I'm at my best on the parts that break in the real world: a phone that loses signal halfway through saving, a payment webhook that fires twice, an AI model that replies in the wrong format.

Today I work on school software running in **117 schools**, most of them on connections that drop several times a day. I own the API layer and the database design behind four apps. Before this I helped take a creator platform from **0 to 10,000+ users** and got its pages loading three times faster.

### Research published on the product I work on

**Two peer-reviewed research papers have been published about the product I build.** One studies the history chatbots — I ship the new features on those; an earlier team built the first version. The other is about how the platform was designed together with teachers, in their own classrooms.

Both papers were written by my colleagues at Shikha, including our founder and my product manager. I didn't write them. My part is the engineering they're written about.

- [Conversations for Learning: Designing Personified Historical Chatbots to Enhance Critical Thinking in K-12 Students](https://doi.org/10.33965/celda2025_202509l042) — CELDA 2025
- [AI-Human Synergy: Using Design Thinking to Build for and with Teachers](https://doi.org/10.1007/978-3-032-29791-4_25) — Springer, 2026

### Where to start

Read these in order. Each README explains how the thing is built, what it promises to always do, and which alternatives I turned down and why.

1. **[claims-processing-system](https://github.com/Saurav02022/claims-processing-system)** — works out what a health insurance claim should actually pay: what's covered, what the deductible eats, what's left. Money maths gets no partial credit, so the calculation is a pure engine with no framework anywhere near it, every claim saves in one all-or-nothing database step, and there is more test code than application code. **Start here — it's the deepest backend work.** · `FastAPI · PostgreSQL`
2. **[rto-shield](https://github.com/Saurav02022/rto-shield)** — when a customer refuses a cash-on-delivery parcel, the seller pays shipping both ways. This puts an AI phone call in between: confirm the order, then dispatch. The hard part is that the call result can arrive two or three times, so the system is built to record it exactly once. · `FastAPI · Next.js · Bolna`
3. **[ai-interview](https://github.com/Saurav02022/ai-interview)** — book a mock interview with credits, take it on a video call that writes its own transcript, and get written feedback once you hang up. The payout to the interviewer is protected in three separate layers so a repeated message can never pay twice. · `Next.js · FastAPI · Stream`
4. **[resume-builder](https://github.com/Saurav02022/resume-builder)** — rewrites your résumé for one specific job. You see every change side by side and approve it before anything is exported to PDF. The AI is locked to a fixed format, so it can't quietly break your layout. · `Next.js · FastAPI` · [try it](https://resume-builder-saurav02022.vercel.app)
5. **[linkedin-hashtag-refresh-engine-app](https://github.com/Saurav02022/linkedin-hashtag-refresh-engine-app)** — a LinkedIn post stops travelling once its hashtags go stale. This drafts three fresh sets and posts your pick as a comment in one click. The real work was LinkedIn's login, which expires every 60 days and had to be renewed by hand in code. · `Next.js` · [try it](https://ai-linkedin-hashtag-refresh-engine-app.vercel.app)
6. **[financial-literacy-assistant](https://github.com/Saurav02022/financial-literacy-assistant)** — budgeting and saving for people starting from zero. Every number is worked out in plain code, never by the AI, so a model outage can change the wording but never the maths. Built in a three-hour hackathon. · `Next.js · Supabase`

### Experience

- **Shikha Learning Labs** — Software Engineer, EdTech, Mumbai. Four apps (web and Android) used across **117 schools**, running **96%+ of the time without a crash**. Background jobs succeeded **98% of the time over 5,000+ submissions**, and the 2% that failed retried safely instead of saving the same thing twice. Schools on weak internet were losing teachers' work, so I made the app save to the phone first and sync when the signal returns — that stopped the losses at **50+ schools**. I also cut a teacher's marking time from **40 minutes to 5–10**.
- **Nuveb** — Full-Stack Developer, Bengaluru. Built the creator side of a video platform as it grew from **0 to 10,000+ users**. Pages were taking **8.5 seconds** to load; I got them to **2.5 seconds** for **50,000+ monthly visitors** by changing how the browse pages fetched their data.

### Open source

I joined Social Winter of Code as a contributor, and came back to the summer round as a mentor.

**Mentor — Social Summer of Code 2026.** Two projects, since June. My job is deciding what gets built, in what order, and what finished actually means — not writing the code myself. Between them the two projects have drawn **41 different contributors**.

- **[EduFlow AI](https://github.com/prabhakarshukla/EduFlow-AI)** (23 contributors, 31 forks) — a study platform with around 100 open tasks for the group. On the harder ones I ask the contributor to write down their approach before they start building.
- **[VidyAI++](https://github.com/jai3546/AI_ROCKERS)** (23 contributors, 35 forks) — an AI tutoring app the group is cleaning up. I wrote **5** of its ~68 open tasks: a missing import that crashed the app, old pages still being served after a new release, 44 type errors the build was ignoring, and a build that fails when a database setting is missing.

**Contributor — Social Winter of Code 2026.** Picked up open tasks in two projects and finished them.

- **[AlgoFi](https://github.com/denshaw-09/AlgoFi)** (11 contributors, 29 forks) — a marketplace for digital collectibles. Two pull requests merged: started on a beginner task, finished on a harder one — the site-wide dark and light theme, made to survive a page reload. **11 files, +419/−226.**
- **[BrowsePing](https://github.com/browseping/browser-extension)** (5 contributors, 15 forks) — a browser extension for browsing together. Built live typing indicators, **8 files, +365/−123** across 6 commits, still open for review. Also broke their dashboard plan into five smaller tasks other people could pick up.

### Stack

TypeScript · Python · SQL — Next.js · React · React Native — FastAPI · Node.js — PostgreSQL · Redis · Firestore · IndexedDB — Google Gemini — Docker · GCP Cloud Run · Vercel · GitHub Actions — Playwright · pytest

### Elsewhere

[Portfolio](https://saurav02022-portfolio.vercel.app) · [LinkedIn](https://linkedin.com/in/saurav02022) · [LeetCode](https://leetcode.com/u/Saurav02022) · sk729584@gmail.com — open to full-stack or AI engineering roles, happy to relocate.
