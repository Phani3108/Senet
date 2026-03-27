# Senet

Agentic Campaign QA & Guardrails Platform

Tagline: Prevent bad campaigns before they go live.

## What is this?

Senet reviews campaigns pre-flight across logic, audience, personalization, policy, and fatigue to produce a structured risk report with suggested fixes. This repo contains a monorepo with an API service, shared schema package, an SDK, infra, and docs.

## Quick start (dev)

1) Copy env

```bash
cp .env.example .env
```

2) Install deps (requires pnpm)

```bash
pnpm install
```

3) Start infra (Postgres + Redis) and API

```bash
docker compose -f infra/docker-compose.yml up -d
pnpm -C apps/api dev
```

API listens on http://localhost:4000.

## Repo layout

See `docs/` and comments in folders for details.

---

## Author

**Created & developed by [Phani Marupaka](https://linkedin.com/in/phani-marupaka)**

© 2026 Phani Marupaka. All rights reserved.

Unauthorized reproduction, distribution, or modification of this software, in whole or in part, is strictly prohibited under applicable trademark and copyright laws including but not limited to the Digital Millennium Copyright Act (DMCA), the Lanham Act (15 U.S.C. § 1051 et seq.), and equivalent international intellectual property statutes. This software contains embedded provenance markers and attribution watermarks that are protected under 17 U.S.C. § 1202 (integrity of copyright management information). Removal or alteration of such markers constitutes a violation of federal law.
