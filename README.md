## Hi, I'm Arvind 👋

I'm a full stack developer based in Hamilton, New Zealand. I mostly work on the
backend in C#/.NET, and I'm happy building the React frontend on top when a project
needs it. Recently finished my Master of IT at the University of Waikato.

I've got around 3 years of experience as a developer, plus an internship here in NZ
where I led a small team building an AI platform for a local software company. These
days I like building things that actually run end to end, so most of what's here is
full projects rather than snippets. APIs, real time features, background jobs, a bit
of AI, and the deployment to make it all work.

### What I work with

- **Backend:** C#/.NET, ASP.NET Core, Entity Framework Core, Python/FastAPI
- **Frontend:** React, Next.js, TypeScript, Tailwind
- **Data & messaging:** PostgreSQL, SQL Server, Redis, RabbitMQ, SignalR
- **Other:** Docker, Cloudflare, Git, and a healthy amount of testing

### A few things I've built

- **[kiwiDeal](https://github.com/erwin09chauhan/kiwiDeal)** ([live demo](https://kiwideal.pages.dev/)) — a marketplace with fixed price listings and live auctions. Built as a modular monolith with six independent modules talking to each other through an outbox based event pipeline, so the boundaries stay clean without the overhead of microservices. Live bidding and notifications run over SignalR, payments go through Stripe checkout, and auction bids handle concurrent writes safely so two people bidding at once can't corrupt the state.

- **[Kiwi Careers Tracker](https://github.com/erwin09chauhan/kiwi-careers-tracker)** ([live demo](https://kiwicareerstracker.pages.dev/)) — a job application tracker that follows each application from applied through to offer or rejection. Every status change fans out through a message queue to independent consumers, one writing the audit log, another pushing a live notification, so the pieces stay decoupled. There's a background service that watches for due reminders and Redis handling caching and rate limiting. Built on Clean Architecture with CQRS.

- **[DocuFlow](https://github.com/erwin09chauhan/docuflow)** ([live demo](https://docu-flow.pages.dev/)) — a multi tenant platform where you upload a PDF, spreadsheet, or contract and get structured fields pulled out of it by AI, with a confidence score per field. Uploads don't block, they get queued and processed in the background through a pipeline of stages. Each tenant's data is fully isolated at the database level, and the AI backend sits behind a single interface so it can be swapped by config rather than code changes.

- **[Airport Admin](https://github.com/erwin09chauhan/airport-admin)** ([live demo](https://airport-admin.pages.dev/)) — a staff scheduling system for airport ground operations. The interesting part is the roster engine, which assigns crew to shifts while respecting a stack of real constraints at once: per person hour limits per day and week, max consecutive days, approved leave, and marked availability. Role based access separates what admins, supervisors, and crew can each see and do.

Find more details in the respective repos. A couple of the demos are on free hosting, so give them a moment to wake up on the first load.

### Get in touch

- 📧 arvindkumar.mularam@gmail.com
- 💼 [LinkedIn](https://linkedin.com/in/arvind-chauhan-515452417)
- 🌐 [Portfolio](https://portfolio-website-9pk.pages.dev)
