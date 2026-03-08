# 🛡️ SVAT (Site Viability Assessment Tool)
### Pursuit AI Fellowship — Level 2 | H2 Intelligence Suite — MVP 3

## What It Does
An AI-powered map-based tool that assesses whether a location 
is viable for green hydrogen production. It scores sites across 
4 pillars: Energy, Water, Policy, and Infrastructure.

## Why We Built It
Finding the right site for a green hydrogen plant requires 
analyzing dozens of data points. SVAT makes that instant.

## Frontend Stack
- Framework: Next.js 14 (App Router)
- UI: Tailwind CSS + Radix UI
- Maps: Mapbox GL JS
- Charts: Recharts + D3.js
- Forms: React Hook Form + Zod
- State: Zustand + React Query
- Auth: Clerk / Auth0
- Deploy: Vercel

## Backend Stack
- Runtime: Node.js + Fastify
- Database: PostgreSQL + PostGIS (via Supabase)
- Cache: Redis via Upstash (6hr TTL)
- Search: Typesense
- PDF Generation: Puppeteer + Handlebars
- Job Queue: BullMQ
- Storage: AWS S3 / Cloudflare R2
- Monitoring: Sentry + Datadog

## Scoring Engine
- 4 pillars scored simultaneously (parallel API calls)
- Weights: Energy 30% | Water 20% | Policy 25% | Infrastructure 25%
- Nightly re-scoring job for saved assessments

## My Contributions 🌟
- 🎨 UX/UI Design — logo design 
- 📋 Product Manager (PM) — wrote the PRD, defined features & user stories
- 🏗️ Program Manager (PgM) — coordinated team, timelines, deliverables
- 💻 Frontend Developer — contributed to the full user-facing interface


## Team
Built with teammates Jawad (backend) and Christian
as part of the Pursuit AI Fellowship L2.
