### Vitor Solen

Solo developer. I build and operate software for businesses that can't afford to stop: point of sale, inventory, ad operations, scheduling.

<br>

**Languages**

<img src="https://skillicons.dev/icons?i=ts,rust,go,py,kotlin,swift,js,bash&perline=8" alt="TypeScript, Rust, Go, Python, Kotlin, Swift, JavaScript, Bash">

**Platforms and tools**

<img src="https://skillicons.dev/icons?i=nodejs,nextjs,react,fastapi,spring,postgres,sqlite,redis,prisma,docker,cloudflare,workers,githubactions,linux&perline=14" alt="Node.js, Next.js, React, FastAPI, Spring, Postgres, SQLite, Redis, Prisma, Docker, Cloudflare, Workers, GitHub Actions, Linux">

<br>

**Architecture I work in**

| Pattern | In practice |
|---|---|
| Offline-first | local-first writes, durable queues, sync on reconnect |
| Multi-tenant | isolation per tenant, down to database and credentials |
| Modular monolith | module boundaries enforced in code (Spring Modulith) |
| Event-driven | webhooks, job queues, idempotent workers |
| Edge and serverless | Cloudflare Workers, D1, static assets at the edge |
| Domain-driven | ubiquitous language per context, decisions as ADRs |
| Infrastructure as code | GitOps, deploys pinned by image digest, automatic rollback |

<br>

**Building**

- **PDV** · offline-first supermarket checkout in Rust. Slint UI, SQLite, NFC-e fiscal receipts. Sells without internet and syncs when the connection returns.
- **NexusPhone** · operations system for Apple resellers: stock per device, repairs, finance, wholesale. Next.js, Postgres, Cloudflare Workers.
- **Horizon** · Meta Ads operations for agencies, with each company isolated down to its credentials. TypeScript, FastAPI, Postgres.
- **rumo** · Claude Code plugin that takes work from ticket to merged PR, behind a review gate tied to the commit being merged.
- **tars** · GitHub App that turns a mention into an approved issue, builds it on a worker and returns the PR.
