## Saurav Kumar

Software engineer, three years in production. I work out what a thing needs to do, design the database, write the API and the app, and put it live myself. On six of my own projects I was the only engineer on all of it. On one, nobody gave me a brief. I wrote the problem statement, decided who it was for, then built it.

Today I work on school software. I own the API behind four apps, web and Android, and I designed the database under all four. A change to one table is a change all four apps have to live with, so that schema gets thought about before it gets written. The apps run in 117 schools. At about 50 of them the connection drops several times a day, so the app saves a teacher's work on the phone first and sends it once the signal comes back.

### What I'm working on now

**Shikha Learning Labs** — Software Engineer, Mumbai. EdTech, used in government and private schools.

I own the API and the database schema behind four apps. The one I have spent most time on is the **AI Teacher Coach**.

Coaching a teacher one to one is the thing that actually improves their teaching. It is also the thing a school can least afford to do, because it needs a trained mentor sitting in the room for the whole class. A sixty-minute class costs a mentor sixty minutes, and the coaching only happens on the days somebody is free to attend.

Now the teacher sets up the class in the app themselves. They start a voice recording when the class begins and stop it at the end. We keep the audio, and the coaching is built from it: what went well, what to work on, and what to try instead next time. It comes back in five to ten minutes, with nobody in the room. The scoring runs on a background queue, so the teacher is not sitting there waiting on it.

We built the web app first, then the Android one. Both are in use. About 400 assessments run through this every week, for 200+ teachers.

The background jobs succeed 98% of the time over 5,000+ submissions. The 2% that fail are the interesting part. They retry on their own, and they are written so that a job which runs twice saves the same result once, not twice. Before that queue existed, schools on bad connections were losing teachers' work outright. Saving on the phone first and syncing later stopped it at 50+ schools.

One bug is worth naming. On Android, unsaved audio was being deleted quietly. Nobody reported it as data loss because nobody knew it had happened. I traced it, and now every file is checked to exist before anything writes over it. That recovered 20+ class recordings.

### Research published on the product I work on

Two peer-reviewed research papers have been published about the product I build. One studies the history chatbots. I ship the new features on those. An earlier team built the first version.

The other is about how the platform was designed together with teachers, in their own classrooms.

Both papers were written by my colleagues at Shikha, including our founder and my product manager. I didn't write them. My part is the engineering they're written about.

- [Conversations for Learning: Designing Personified Historical Chatbots to Enhance Critical Thinking in K-12 Students](https://doi.org/10.33965/celda2025_202509l042) — CELDA 2025
- [AI-Human Synergy: Using Design Thinking to Build for and with Teachers](https://doi.org/10.1007/978-3-032-29791-4_25) — Springer, 2026

### Before this

**Nuveb** — Full-Stack Developer, Bengaluru. A video platform for creators, which grew from nothing to 10,000+ creators while I was there. I built the creator side: video, scheduling, payments.

Pages were taking 8.5 seconds to load for 50,000+ monthly visitors. The browse pages were rebuilding themselves on every single request, for content that barely changed. I moved them to pre-built pages and kept the rebuild only where the page was personal to the user. That took it to 2.5 seconds. Separately, image requests were sitting at 3.2 seconds across 10,000+ items. Profiling pointed at the resizing step, so I moved that work to the server. 1.9 seconds after.

### Things I built on my own

Read these in order. Each README says how it is built, what it always guarantees, and which alternatives I turned down.

1. **[claims-processing-system](https://github.com/Saurav02022/claims-processing-system)** — works out what a health insurance claim should actually pay. What is covered, what the deductible takes, what is left. Money maths gets no partial credit, so the calculation is a pure engine with no framework near it, and a claim either saves completely or not at all. There is more test code than application code. **Start here. It is the deepest backend work.** `FastAPI · PostgreSQL`
2. **[rto-shield](https://github.com/Saurav02022/rto-shield)** — when a customer refuses a cash-on-delivery parcel, the seller pays shipping both ways. This puts an AI phone call in between. Confirm first, dispatch after. Nobody gave me this brief. I wrote the problem statement, picked the users, chose the stack, then built it. The hard part is that the call result can arrive two or three times, so it is built to record it exactly once. `FastAPI · Next.js · Bolna`
3. **[ai-interview](https://github.com/Saurav02022/ai-interview)** — book a mock interview with credits, take it on a video call that writes its own transcript, get written feedback once you hang up. The payout to the interviewer is protected in three separate places, so a repeated message can never pay twice. `Next.js · FastAPI · Stream`
4. **[resume-builder](https://github.com/Saurav02022/resume-builder)** — rewrites your résumé for one specific job. You see every change side by side and approve it before anything exports. The AI is locked to a fixed shape, so it cannot quietly break your layout. `Next.js · FastAPI` · [try it](https://resume-builder-saurav02022.vercel.app)
5. **[linkedin-hashtag-refresh-engine-app](https://github.com/Saurav02022/linkedin-hashtag-refresh-engine-app)** — a post stops travelling once its hashtags go stale. This drafts three fresh sets and posts your pick as a comment. I first tried to read the post automatically. It kept breaking, and the reliable fix cost money, so I dropped it and let people paste the text instead. The login was the real work: LinkedIn expires it every 60 days and it had to be renewed by hand in code. `Next.js` · [try it](https://ai-linkedin-hashtag-refresh-engine-app.vercel.app)
6. **[financial-literacy-assistant](https://github.com/Saurav02022/financial-literacy-assistant)** — budgeting and saving for people starting from zero. Every number is worked out in plain code, never by the AI, so a model outage can change the wording but never the maths. Built in a three-hour hackathon. `Next.js · Supabase`

### Open source

I joined Social Winter of Code as a contributor and came back to the summer round as a mentor.

**Mentor, Social Summer of Code 2026.** Two projects, since June. I decide what gets built, in what order, and what finished means. I do not write the code. Between them the two projects have drawn 41 different contributors.

- **[EduFlow AI](https://github.com/prabhakarshukla/EduFlow-AI)** (23 contributors, 31 forks) — a study platform with around 100 open tasks. On the harder ones I ask the contributor to write down their approach before they start building.
- **[VidyAI++](https://github.com/jai3546/AI_ROCKERS)** (23 contributors, 35 forks) — an AI tutoring app the group is cleaning up. I wrote 5 of its 68 open tasks: a missing import crashing the app, old pages still served after a release, 44 type errors the build was ignoring, and a build that fails when one database setting is absent.

**Contributor, Social Winter of Code 2026.** Picked up open tasks in two projects and finished them.

- **[AlgoFi](https://github.com/denshaw-09/AlgoFi)** (11 contributors, 29 forks) — a marketplace for digital collectibles. Two pull requests merged. Started on a beginner task, finished on a harder one: the site-wide dark and light theme, made to survive a reload. 11 files, +419/−226.
- **[BrowsePing](https://github.com/browseping/browser-extension)** (5 contributors, 15 forks) — a browser extension for browsing together. Live typing indicators, 8 files, +365/−123 across 6 commits, still open for review. I also broke their dashboard plan into five smaller tasks other people could pick up.

### Stack

TypeScript · Python · SQL — Next.js · React · React Native — FastAPI · Node.js — PostgreSQL · Redis · Firestore · IndexedDB — Google Gemini — Docker · GCP Cloud Run · Vercel · GitHub Actions — Playwright · pytest

### Elsewhere

B.Sc. Mathematics (Honours). Starting an MCA at IIIT Ranchi in 2026.

[Portfolio](https://saurav02022-portfolio.vercel.app) · [LinkedIn](https://linkedin.com/in/saurav02022) · [LeetCode](https://leetcode.com/u/Saurav02022) · sk729584@gmail.com

Looking for a Software Engineer II role, happy to relocate.
