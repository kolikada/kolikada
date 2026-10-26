```console
$ whoami

Full-stack developer who ships the whole thing — the front end,
schema underneath it, the API in between, and the
Ubuntu box the whole lot runs on.

I build AI-augmented SaaS and business systems for small
businesses, keep production hosting infrastructure online for
paying clients, and write the bots and mods that keep a gaming
community running. Most days I'm pair-programming with an AI
agent — I treat it like a fast junior: I own the architecture,
the security model, and the review.
```
### stack

```
lang     typescript · javascript · php · python · bash · sql
web      next.js (app router) · react · vite · tailwind · laravel · twig
api      node · express · hono · fastapi · rest · websockets / socket.io
mobile   expo / react native
data     postgresql · supabase — auth, rls, realtime, edge fns
         prisma · drizzle · sqlite · pg_cron
ml       scikit-learn · predictive analytics · recommendations
infra    ubuntu · docker · nginx · cloudflare · vercel · coolify
         digitalocean · fly.io · bare metal · pnpm monorepos
hosting  pelican · hestia · fossbilling · paymenter
ci/cd    git · github actions · gitea · preview deployments
test     playwright (e2e)
ai       claude api · claude code · mcp · agent harnesses
         gemini · antigravity · cursor · codex
sec      oauth 2.0/pkce · postgres rls · aes-256-gcm · totp
         owasp · rate limiting · turnstile · secrets mgmt
pay      gcash · qr ph · paymongo · stripe
```

### what i build

```diff
+ multi-tenant client portals
    One surface where clients track projects, milestones and
    invoices, with a role-gated staff console beside it. An
    AES-256-GCM credentials vault behind TOTP two-factor (AAL2 +
    recent-auth freshness), a session manager with per-device
    revocation, realtime + daily email digest notifications.
    Every read and write is authorized server-side through
    Postgres RLS — never trusted to the client.

+ llm support automation
    Swapped a helpdesk's built-in AI assistant for a custom
    Claude API integration so client support answers itself
    first and hands off to humans cleanly.

+ hosting automation — billing to provisioning
    Wired billing software to the game-server panel so servers
    provision, suspend and delete off payment status, and tied
    web hosting, game hosting and billing into one onboarding
    flow. Manual provisioning went from hours to minutes, and
    billing-to-service mismatches stopped happening.

+ local payment rails
    Payment gateways on GCash and QR Ph for PHP-denominated
    subscription billing — the gap where Stripe has no
    official Philippine support.

+ multi-app business systems
    One monorepo, one Supabase backend, several independently
    deployed apps (customer site, admin, sales, staff) behind a
    single unified login with role-based routing.

+ adaptive learning platform
    Multi-role LMS (admin, tutor, student, guest) with
    personalized learning paths. Node API owns auth and data;
    a stateless Python ML service handles predictive academic
    monitoring and content recommendations.

+ offline-first point of sale
    Staff run on a React Native app talking to a backend on the
    shop's own LAN, so the shop keeps working when the internet
    doesn't; the public ordering site syncs through Postgres.

+ sales analytics & forecasting
    Web platform for tracking sales performance with AI-driven
    analytics and demand forecasting.

+ websites & event systems
    Marketing sites with multi-step project intake, real email
    delivery and spam protection; private invitation pages with
    per-guest links and RSVPs that fan out to email and Sheets.

+ discord bots & game mods
    Ticketing with transcripts, live server-status embeds, a
    community bounty/rewards system with audit logging, an
    encrypted transaction proxy with role-based access, and
    custom Project Zomboid server mods.

+ agent tooling
    Custom skills, plugins, themes and MCP setups for AI coding
    agents — the scaffolding that makes the AI-assisted workflow
    above actually reliable.
```

### how i work

```console
$ ls -la ~/repos

# most of the good stuff sits behind drwx------ — client and
# company work under NDA. happy to walk through any of it.
```
