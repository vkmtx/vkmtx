### Vitor Solen

Solo developer. Product, code and production, one person.

<img src="https://skillicons.dev/icons?i=ts,rust,go,py,kotlin,swift,js,bash&perline=8" alt="TypeScript, Rust, Go, Python, Kotlin, Swift, JavaScript, Bash">

<img src="https://skillicons.dev/icons?i=nodejs,nextjs,react,fastapi,spring,postgres,sqlite,redis,prisma,docker,cloudflare,workers,githubactions,linux&perline=14" alt="Node.js, Next.js, React, FastAPI, Spring, Postgres, SQLite, Redis, Prisma, Docker, Cloudflare, Workers, GitHub Actions, Linux">

<br>

#### Systems

**PDV** · Rust  
Supermarket checkout that keeps selling with the internet down. Sales commit locally to SQLite and sync when the link returns; NFC-e fiscal keys and QR codes are generated offline. Keyboard-driven Slint UI. 9-crate workspace, 764 tests.

**NexusPhone** · TypeScript, Cloudflare  
ERP for Apple resellers: stock per device, repairs, finance, wholesale. Each store runs on its own Durable Object as its database, so one store cannot reach another's data. 30 ADRs, 864 test files.

**Horizon** · TypeScript, Python  
Meta Ads operations for agencies. FastAPI API and gateway, background worker, Next.js console. Every company is isolated down to its Meta credentials.

**rumo** · Claude Code plugin  
Ticket, plan, build, review, merge. 9 typed agents, and a merge gate that refuses anything whose reviewed commit is not HEAD.

**tars** · TypeScript, GitHub App  
Turns a mention into an issue with acceptance criteria, waits for approval, dispatches the build to a worker machine and replies with the PR.

**Infrastructure**  
35 service stacks behind Traefik, declared in one repo. Deploys pinned by image digest, automatic rollback on failed health checks.

<br>

#### How the work is built

| Pattern | In practice |
|---|---|
| Offline-first | local commit, durable queue, sync on reconnect |
| Tenant isolation | one database per tenant, enforced below the application |
| Modular monolith | module boundaries checked in code (Spring Modulith) |
| Event-driven | webhooks, job queues, idempotent workers |
| Edge | Cloudflare Workers, Durable Objects, D1 |
| Domain-driven | a glossary per project, 269 ADRs across repos |
