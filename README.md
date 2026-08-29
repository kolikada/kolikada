```
┌──────────────────────────────────────────────────┐
│                                                  │
│   Kenneth M. Tañeza                              │
│   full-stack · ai integration · infrastructure   │
│                                                  │
│   san jose del monte, bulacan, philippines       │
│                                                  │
└──────────────────────────────────────────────────┘
```

```console
$ whoami

Full-stack developer who ships the whole thing — the Next.js
front end, the Postgres schema underneath it, and the Ubuntu
box the whole lot runs on.

I build AI-augmented SaaS for small businesses, and I keep
production hosting infrastructure online for paying clients
across the Philippines.
```

```console
$ cat ./now

k-made solutions      founder & lead developer      2026 →
                      multi-tenant saas/paas for small
                      businesses on next.js, supabase, vercel

tekkura               head developer                2025 →
                      game hosting & server infrastructure,
                      bare metal + vps fleet, full devops

the last of zomboid   lead dev & community manager  2025 →
                      discord.js bots, pz server mods,
                      community ops
```

### stack

```
lang     typescript · javascript · php · python · bash · sql
web      next.js (app router) · react · laravel · twig
data     postgresql · supabase — auth, rls, realtime, edge fns
infra    ubuntu · docker · nginx · cloudflare · vercel
         digitalocean · fly.io · bare metal
ci/cd    git · github actions · gitea · preview deployments
ai       claude api · claude code · mcp · gemini · cursor
sec      oauth 2.0/pkce · postgres rls · aes-256-gcm · totp
         owasp · rate limiting · turnstile · secrets mgmt
```

### where the hours go

```console
$ time-spent --since 2025

next.js / react       ███████████████████░░░░░░░░░
supabase / postgres   ████████████████░░░░░░░░░░░░
linux / devops        █████████████░░░░░░░░░░░░░░░
php / laravel         ██████████░░░░░░░░░░░░░░░░░░
claude api / agents   ████████░░░░░░░░░░░░░░░░░░░░
discord.js            ████░░░░░░░░░░░░░░░░░░░░░░░░
```

### deployed

```diff
+ k-made client portal — multi-tenant saas
    One surface where clients track projects, milestones and
    invoices, plus a role-gated staff admin console beside it.
    AES-256-GCM credentials vault behind TOTP two-factor
    (AAL2 + recent-auth freshness), a session manager with
    per-device revocation, and realtime + email digest
    notifications via Vercel Cron and Resend. Every read and
    write is authorized server-side through Postgres RLS —
    never trusted to the client.

+ claude × chatwoot — llm support automation
    Replaced Chatwoot's built-in AI assistant with a custom
    Anthropic Claude API integration, built end to end with
    Claude Code, powering support automation for clients.

+ fossbilling × pelican × hestia — hosting ecosystem
    Custom integration module wiring FOSSBilling to Pelican
    Panel so game servers provision, suspend and delete off
    billing status. Cut manual provisioning from hours to
    minutes and killed the billing-to-service mismatches.

+ gcash & qr ph payment gateway
    Payment gateway for FOSSBilling on Philippine rails,
    automating PHP-denominated subscription billing where
    Stripe has no official support.

+ unknown operator & black market — discord.js bots
    A community bounty and rewards system with admin tooling
    and audit logging, and an encrypted transaction proxy
    with role-based access and tamper-resistant storage.
```

```console
$ ls -la ~/repos

# most of the good stuff sits behind drwx------ — client and
# company work under NDA. happy to walk through any of it.
```

```console
$ cat contact.txt

email     tanezakennethm@gmail.com
github    github.com/kolikada
based     bulacan, philippines · utc+8
langs     english (professional) · filipino (native)
```
