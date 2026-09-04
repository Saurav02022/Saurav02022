# Saurav Kumar

I am an applied AI engineer in Mumbai. I run LLM systems in production and I build the whole product around them.

I came to the AI work from full stack work on the same products, so I still build the whole thing: Python, FastAPI, TypeScript, React, Next.js and PostgreSQL.

I am open to AI Engineer, Applied AI Engineer, GenAI Engineer, Forward Deployed Engineer and Software Engineer II roles.

Email: [sk729584@gmail.com](mailto:sk729584@gmail.com)  
Portfolio: [saurav02022.github.io](https://saurav02022.github.io)  
LinkedIn: [linkedin.com/in/saurav02022](https://linkedin.com/in/saurav02022)

## What I Do

- Build LLM systems that make a real decision, so a person checks the output instead of producing all of it.
- Measure what the model decides against human judgement, and gate every change on that number.
- Keep LLM cost and latency down with response caching and queued inference.
- Build the whole stack around it on FastAPI, PostgreSQL, Redis and Next.js, including CI/CD and deployment.
- Build offline-safe flows for schools where the internet is weak, so nothing is lost when the connection drops.

## Current Work: Shikha Learning Labs

[Shikha Learning Labs](https://shikha.ai) is an EdTech initiative of the Shantilal Shanghvi Foundation. We build digital products for schools, teachers, students, principals and school admins.

I work as a Software Engineer. Our products are used across 117 schools. I am the sole engineer for 4 of 10 web products and I also work on shared parts of the platform.

My work includes:

- Built a rubric-scored analyser that takes the first pass on student submissions, around 5,000 a month from 300+ students. It returns approve, reject or a comment, so teachers cross-check instead of reading every one.
- Measure that analyser against teacher judgement instead of assuming it is right. Agreement is 7 in 10 today, and every prompt, model and model-config change is tested against that number before release.
- Built the AI feedback workflow for classroom audio on FastAPI workers and Redis queues. It runs 400+ classes a week for 200+ teachers and brings a mentor's review of one class from around 60 minutes to 5-10 minutes.
- Keep LLM cost flat with a response cache keyed on a SHA-256 hash of the scores, the prompt version and the model, so a result is recomputed only when one of those changes.
- Moved the team to token-based deploys from GitHub Actions across 12 projects, so six engineers ship from one paid Vercel seat and we save about $1,200 a year.
- Built offline-safe recording with IndexedDB for around 50 rural schools, so no class audio is lost when the connection drops.
- Built shared UI components, single login and role-based access used across products, so everyone gets the right access.

## Research Connected To My Product Work

Two research papers from the Shikha team are connected to products I built or worked on.

These papers were written by Shikha's founder, product managers, researchers and wider team members. I am not listing myself as an author. My connection is through the engineering and product work behind these tools.

- [AI-Human Synergy: Using Design Thinking to Build for and with Teachers](https://doi.org/10.1007/978-3-032-29791-4_25)  
  Related to our AI teacher workflow and multi-assistant platform for teachers.

- [Conversations for Learning: Designing Personified Historical Chatbots to Enhance Critical Thinking in K-12 Students](https://doi.org/10.33965/celda2025_202509l042)  
  Related to AI chatbot work for K-12 learning and student questioning.

## Previous Work: Nuveb

Nuveb is an open OTT network for creators. It helps creators publish video content and earn from it without depending only on large platforms.

I worked as a Full Stack Developer across the viewer-facing OTT platform and the creator side of the product.

My work included:

- Built creator portal features used by 10,000+ creators.
- Built multi-step video upload, publishing, scheduling and payment flows.
- Improved key OTT page load time from 8.5 seconds to 2.5 seconds for 50,000+ monthly users.
- Reduced image API response time from 3.2 seconds to 1.9 seconds across 10,000+ catalogue items.

## Projects

- [rto-shield](https://github.com/Saurav02022/rto-shield)  
  An ops console where an AI voice call confirms a cash-on-delivery order before it ships. The provider reports the same call up to three times, so one idempotent mutator keyed on the call ID decides the order state and a repeat can never ship a second parcel.

- [claims-processing-system](https://github.com/Saurav02022/claims-processing-system)  
  A health-insurance payout engine. The rules are about 170 lines of plain Python with nothing from the web framework in them, covered by 74 tests, and the whole claim write sits inside one PostgreSQL function.

- [chat-ai-app](https://github.com/Saurav02022/chat-ai-app)
  A streaming chat app built on the Vercel AI SDK with OpenAI models. I have kept working on it since November 2024 — 208 commits across 201 separate days.

- [ai-interview](https://github.com/Saurav02022/ai-interview)  
  A mock interview platform with video calls, transcripts and AI feedback.

- [resume-builder](https://github.com/Saurav02022/resume-builder)  
  A resume tailoring tool for one job, with changes shown side by side. [Try it](https://resume-builder-saurav02022.vercel.app)

- [linkedin-hashtag-refresh-engine-app](https://github.com/Saurav02022/linkedin-hashtag-refresh-engine-app)  
  A small tool that drafts hashtag sets for LinkedIn posts. [Try it](https://ai-linkedin-hashtag-refresh-engine-app.vercel.app)

- [financial-literacy-assistant](https://github.com/Saurav02022/financial-literacy-assistant)  
  A budgeting assistant for beginners, built in a three-hour hackathon.

## Open Source And Learning

- Mentored 41 contributors across the open-source projects EduFlow AI and VidyAI++ at Social Summer of Code 2026, and filed 5 tracked issues on VidyAI++ including 44 TypeScript errors the build was hiding.
- Contributed at Social Winter of Code 2026, with light and dark theming across 11 files in AlgoFi.
- Solved 200+ DSA problems on LeetCode and takeUforward. LeetCode contest rating: 1,616.

## Tech Stack

**AI and LLM systems:** LLM evaluation, prompt engineering, structured outputs, response caching, queued inference, AI voice agents, LLM APIs (OpenAI, Gemini, DeepSeek).

**Languages:** Python, TypeScript, JavaScript, SQL.

**Backend:** FastAPI, Node.js, REST APIs, Redis, message queues, pytest.

**Frontend:** React, Next.js, Tailwind CSS.

**Databases and infrastructure:** PostgreSQL, Supabase, Firestore, Docker, GitHub Actions, CI/CD, GCP, Google Cloud Run, Vercel, Sentry, monitoring and observability.

## Education

- MCA, Artificial Intelligence and Machine Learning, Indian Institute of Information Technology Ranchi, 2026-2028 expected
- Full-Stack Web Development, Masai School, 2022-2023, GPA 9/10
- B.Sc. Mathematics (Honours), Munger University, 2019-2022

[Portfolio](https://saurav02022.github.io) · [LinkedIn](https://linkedin.com/in/saurav02022) · [LeetCode](https://leetcode.com/u/Saurav02022) · [Email](mailto:sk729584@gmail.com)
