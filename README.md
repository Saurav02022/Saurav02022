# Saurav Kumar

I build web and Android products end to end: the screens people use, the server behind them, the database underneath, and the pipeline that puts it all live. Three years in production, Mumbai.

At [Shikha Learning Labs](https://shikha.ai) in Mumbai I work on [Sakhee](https://shikha.ai), software for schoolteachers running in 117 schools. Before that, Nuveb in Bengaluru.

**Open to a Software Engineer II role, and happy to relocate.** sk729584@gmail.com

## What I have shipped at work

At Shikha, in order of how much of it is mine:

- **The teacher coaching app on Android**, alone, from the first screen to the Play Store listing and the testing with teachers. Assessing a teacher used to need a mentor sitting through the whole class, so a sixty-minute class cost a mentor sixty minutes and only happened when someone was free. Now teachers record the class themselves and get feedback in five to ten minutes. Around 200 teachers use it, most recording two classes a week.
- **The database under all four Sakhee apps.** A change to one table is a change all four have to live with, so that schema gets argued about before anyone writes it.
- **The school calendar**, which I later pulled out into its own service so every app asks it instead of keeping its own copy of the dates.
- **The Google Drive sync**, where a teacher's files move both ways with every version kept. It waits for a pause in the typing before saving, so an hour of editing leaves one version and not forty.
- **The build and deploy pipelines** for all four services.
- **A student portfolio portal**, web and Android, and **an institute website** with an admin area where staff edit their own content. Both alone.
- **The front end of a school quality platform** a state authority uses, with two colleagues.

At Nuveb, the creator side of a video platform, zero to 10,000 creators. The browse pages took 8.5 seconds for 50,000+ monthly visitors because they rebuilt themselves on every request for content that hardly ever changed. Pre-building them brought it to 2.5 seconds. Images went from 3.2s to 1.9s once I profiled them and moved the resizing to the server.

## Things I built on my own

Each repo's README says how it works, what it guarantees, and what I decided against.

- **[claims-processing-system](https://github.com/Saurav02022/claims-processing-system)** — decides what a health insurance claim pays out. More test code than application code. Start here.
- **[rto-shield](https://github.com/Saurav02022/rto-shield)** — an AI voice call confirms a cash-on-delivery order before it ships. Nobody gave me the brief; I wrote it.
- **[ai-interview](https://github.com/Saurav02022/ai-interview)** — mock interviews on a video call that transcribes itself, with feedback after.
- **[resume-builder](https://github.com/Saurav02022/resume-builder)** — rewrites a résumé for one job, every change shown side by side. [try it](https://resume-builder-saurav02022.vercel.app)
- **[linkedin-hashtag-refresh-engine-app](https://github.com/Saurav02022/linkedin-hashtag-refresh-engine-app)** — drafts three hashtag sets and comments your pick. [try it](https://ai-linkedin-hashtag-refresh-engine-app.vercel.app)
- **[financial-literacy-assistant](https://github.com/Saurav02022/financial-literacy-assistant)** — budgeting for beginners. Built in a three-hour hackathon.

Six projects, and on every one of them I was the only engineer: design, frontend, backend, schema, deployment. Mostly Python and TypeScript, FastAPI and Next.js, PostgreSQL on top.

## The bug I think about

On the Android coaching app, unsaved recordings were being deleted without a trace. Nobody had reported it, because nobody knew. The audio was not failing to upload; it was already gone by the time the upload started. Those recordings are the whole product. Now every file has to prove it exists before anything is allowed to write over it.

## Open source

Mentor at Social Summer of Code 2026 for [EduFlow AI](https://github.com/prabhakarshukla/EduFlow-AI) and [VidyAI++](https://github.com/jai3546/AI_ROCKERS), 41 contributors between them. I decide what gets built and what counts as done. I came to it the other way round, as a contributor in the winter round, where I merged the dark and light theme into [AlgoFi](https://github.com/denshaw-09/AlgoFi).

## Elsewhere

Two papers came out of the Sakhee work, [CELDA 2025](https://doi.org/10.33965/celda2025_202509l042) and [Springer CCIS 2026](https://doi.org/10.1007/978-3-032-29791-4_25). Colleagues wrote them; my part is the engineering. B.Sc. Mathematics (Honours), Munger University. Currently doing an MCA at IIIT Ranchi on weekends.

[Portfolio](https://saurav02022-portfolio.vercel.app) · [LinkedIn](https://linkedin.com/in/saurav02022) · [LeetCode](https://leetcode.com/u/Saurav02022) · sk729584@gmail.com
