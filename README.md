# Alexey Orlov

**Frontend-focused fullstack developer · 4 years of commercial experience**

I build web applications with Vue 3 and TypeScript: complex SPAs, real-time interfaces over WebSockets, PWAs. About 30% of my work has been backend — PHP (Symfony) with PostgreSQL and Redis. I care about clear architecture (Feature-Sliced Design), strict typing and business logic covered by tests. In pet projects I also work with Node.js (Fastify), React and LLM APIs.

Remote or hybrid

[![Stack](https://skillicons.dev/icons?i=vue,ts,pinia,svelte,vite,vitest,tailwind,php,symfony,postgres,redis,docker&perline=12)](#tech-stack)

## Work experience

**[Wahelp](https://wahelp.ru)** · July 2022 — July 2026

A marketing automation platform that brings a business's conversations with customers from WhatsApp, Telegram, Instagram and marketplace reviews into a single inbox, integrated with amoCRM and YCLIENTS. Thousands of active businesses, over 3.2M messages processed.

- **Performance.** Cut load time of key sections by 40–45% (from ~3.2 s to ~1.8 s) with a caching strategy and parallel requests on TanStack Query. Improved perceived speed by ~70% with optimistic updates and instant cached data when switching tabs
- **AI in the product.** Built the client side of incoming message analysis and AI-suggested replies in the messenger and CRM, cutting operator response time by about a third
- **Product from scratch.** As the sole frontend developer, designed and launched a loyalty card product built on Feature-Sliced Design
- **UI kit.** ~40 components in Vue and Svelte, adopted across several company projects. Led a full migration of the product from one UI kit to another
- **Migrations.** Legacy PHP templates and jQuery → Vue 3. Options API → Composition API with business logic moved into testable modules, which cut frontend incidents several-fold. Vuex → Pinia without pausing feature work
- **Fullstack.** End-to-end notification system: Vue frontend, PHP Symfony backend. Maintenance notices reduced the support load; promotional campaigns increased sales for the platform's customers
- **Real-time and SSR.** Live updates in the messenger and trigger-based actions in CRM pipelines over WebSockets. SSR with SvelteKit for company landing pages
- **Team.** Code review, task estimation, mentoring junior and fullstack developers. Rolled out Cursor and Claude Code across the team: set up the environment, wrote usage guidelines, trained developers

Work code lives in the company's private repositories; this profile shows my pet projects.

## Pet projects

### [job-radar](https://github.com/Alexsey215/job-radar) — a Telegram bot that finds job postings and scores them against my resume with an LLM

- Collects postings from public Telegram channels and from chats with job aggregator bots (userbot via MTProto / GramJS)
- Claude Haiku filters out posts that aren't job offers, then a single batch call scores each posting from 0 to 100 against several resume profiles at once and explains the score
- Sources sit behind a `VacancySource` interface: when HeadHunter shut down its job-seeker API, the project moved to Telegram without rewriting the core
- Deduplication, favorites and token usage tracking right in the chat

`Node.js` `TypeScript (strict, ESM)` `Fastify` `grammY` `GramJS` `PostgreSQL` `Drizzle ORM` `Anthropic SDK` `Docker` `Vitest`

### [tg-chat](https://github.com/Alexsey215/tg-chat) · [live demo](https://alexsey215.github.io/tg-chat/) — a web client for Telegram messaging via GREEN-API

- Feature-Sliced Design architecture: `entities` → `features` → `widgets` → `pages`
- Receives messages via long polling with automatic reconnection and a connection-lost warning
- Delivery statuses (sending / sent / failed) with retry; incoming messages deduplicated by `idMessage`

`React 19` `TypeScript` `Zustand` `Tailwind CSS 4` `shadcn/ui` `Vite` `Vitest`

## Tech stack

| | |
|---|---|
| **Frontend** | Vue 3 (Composition API), TypeScript, Pinia, TanStack Query, Svelte / SvelteKit (SSR), React, Zustand, Vite, Tailwind, Feature-Sliced Design, PWA |
| **Backend** | PHP (Symfony), Node.js (Fastify), PostgreSQL, Redis, Drizzle ORM, REST API, WebSockets, Telegram bots (grammY) |
| **Mobile** | React Native (maintained the company's mobile app) |
| **Testing & tooling** | Vitest, Jest, Docker, CI/CD (Gitea, GitHub Actions) |
| **AI** | AI features in the product UI, Claude API, Cursor, Claude Code |

## Contact

Telegram: [@Alexsey1509](https://t.me/Alexsey1509)
