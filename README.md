# Saurav Kumar

Software engineer, three years in production. Mumbai, India. Python and TypeScript, FastAPI and Next.js, PostgreSQL. Looking for a Software Engineer II role, happy to relocate. sk729584@gmail.com

I work out what a thing needs to do, design the database, write the API and the app, and put it live myself. On six of my own projects I was the only engineer on all of it. On one, nobody gave me a brief — I wrote the problem statement, decided who it was for, then built it.

## Now — Shikha Learning Labs, Mumbai (Nov 2024 – present)

Shikha Labs builds [Sakhee](https://shikha.ai), an AI tool for schoolteachers. I am one of the engineers on it. I own the API behind four apps, web and Android, and I designed the database under all four — a change to one table is a change all four have to live with, so that schema gets argued about before it gets written.

**The Android app for the teacher coach is mine end to end**, including the release and the testing with teachers. Assessing how a teacher taught used to mean a mentor sitting through the whole class: a sixty-minute class cost a mentor sixty minutes, and it only happened when a mentor was free. Now the teacher records the class themselves and the feedback comes back in five to ten minutes, with nobody in the room. Around 200 teachers use it, most recording at least two classes a week.

Those recordings are the product, so losing one is the worst thing that can happen. On Android, unsaved audio was being deleted silently — nobody reported it, because nobody knew. The recordings were not failing to upload; they were gone before the upload was attempted. I traced it and made every file prove it exists before anything writes over it.

Two other parts of Sakhee are mine, both written alone. The school calendar, which I later pulled into its own service so every app asks it instead of keeping its own copy of the dates. And the Google Drive link: a teacher's files sync both ways with every version kept, and it waits for a pause in the typing before it saves. An hour of editing leaves one version, not forty. The build and deploy pipelines for our four services are mine too.

I also build whole products on my own here — a student portfolio portal, web and Android, and an institute website with an admin area where staff edit their own content. And with two colleagues, the front end of a platform a state authority uses to check school quality.

Two peer-reviewed papers have been published on this work — [CELDA 2025](https://doi.org/10.33965/celda2025_202509l042) and [Springer CCIS 2026](https://doi.org/10.1007/978-3-032-29791-4_25). Colleagues wrote them, including our founder and my product manager. My part is the engineering.

## Before — Nuveb, Bengaluru (May 2023 – Sep 2024)

Built the creator side of a video platform as it grew from nothing to 10,000+ creators. Pages were taking 8.5 seconds for 50,000+ monthly visitors because the browse pages rebuilt themselves on every request, for content that barely changed. Moving them to pre-built pages took it to 2.5 seconds. Image requests went 3.2s to 1.9s once I profiled them and moved the resizing to the server.

## Things I built on my own

Each README says how it is built, what it always guarantees, and which alternatives I turned down.

1. **[claims-processing-system](https://github.com/Saurav02022/claims-processing-system)** — works out what a health insurance claim should pay. The money maths is plain Python with nothing from the web framework in it, and a claim saves completely or not at all. More test code than application code. **Start here.** `FastAPI · PostgreSQL`
2. **[rto-shield](https://github.com/Saurav02022/rto-shield)** — an AI voice call confirms a cash-on-delivery order before dispatch. Nobody gave me the brief. The phone service reports the same call up to three times, so one handler matches on the call ID and the parcel ships only on a real confirmation. `FastAPI · Next.js`
3. **[ai-interview](https://github.com/Saurav02022/ai-interview)** — book a mock interview, take it on a video call that writes its own transcript, get written feedback after. A repeated message updates the same booking instead of paying the interviewer twice. `Next.js · FastAPI`
4. **[resume-builder](https://github.com/Saurav02022/resume-builder)** — rewrites a résumé for one job, every change shown side by side before export. The model is locked to a fixed shape so it cannot quietly break the layout. `Next.js · FastAPI` · [try it](https://resume-builder-saurav02022.vercel.app)
5. **[linkedin-hashtag-refresh-engine-app](https://github.com/Saurav02022/linkedin-hashtag-refresh-engine-app)** — drafts three hashtag sets and posts your pick as a comment. I dropped automatic post-reading when the reliable fix cost money. `Next.js` · [try it](https://ai-linkedin-hashtag-refresh-engine-app.vercel.app)
6. **[financial-literacy-assistant](https://github.com/Saurav02022/financial-literacy-assistant)** — budgeting for beginners, where every number is worked out in plain code and the model only writes the wording. Three-hour hackathon. `Next.js · Supabase`

## Open source

I joined Social Winter of Code as a contributor and came back to the summer round as a mentor.

**Mentor, Social Summer of Code 2026** — two projects, 41 contributors between them. I decide what gets built and what finished means. On [EduFlow AI](https://github.com/prabhakarshukla/EduFlow-AI) I ask contributors to write down their approach before they start. On [VidyAI++](https://github.com/jai3546/AI_ROCKERS) I wrote 5 of the open tasks: a missing import crashing the app, stale pages served after a release, 44 type errors the build ignored, and a build that fails without one database setting.

**Contributor, Social Winter of Code 2026** — merged the site-wide dark and light theme into [AlgoFi](https://github.com/denshaw-09/AlgoFi) and made it survive a reload. Added live typing indicators to [BrowsePing](https://github.com/browseping/browser-extension), still open for review.

## Stack

TypeScript · Python · SQL — Next.js · React · React Native — FastAPI · Node.js — PostgreSQL · Redis · Firestore · IndexedDB — Google Gemini — Docker · GCP Cloud Run · Vercel · GitHub Actions — Playwright · pytest

## Elsewhere

B.Sc. Mathematics (Honours), Munger University, 2019–2022. MCA at IIIT Ranchi, 2026–2028, weekends alongside work.

[Portfolio](https://saurav02022-portfolio.vercel.app) · [LinkedIn](https://linkedin.com/in/saurav02022) · [LeetCode](https://leetcode.com/u/Saurav02022) · sk729584@gmail.com
