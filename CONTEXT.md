# Project Context

## Purpose

This file is the handoff note for future coding sessions. Keep it current whenever implementation status, decisions, blockers, commands, dependencies, routes, or next steps change.

## Current State

- The repository is currently a planning scaffold for Ahmad Saladin's personal website v0.
- Source brief exists in `brief.md`.
- Agent instructions exist in `AGENTS.md`.
- Reusable design guidance exists in `DESIGN.md`.
- Detailed implementation plan exists in `IMPLEMENTATION_PLAN.md`.
- Astrofy has not yet been installed in this repo.
- No application source files have been created yet.

## Source Of Truth

- `brief.md`: full product brief and content requirements.
- `AGENTS.md`: concise rules future agents should follow.
- `DESIGN.md`: reusable design rules for consistency across pages.
- `IMPLEMENTATION_PLAN.md`: phased build plan and acceptance checklist.

## Key Decisions

- Use Astrofy as the base template.
- Keep Astrofy's useful Astro, Tailwind, portfolio, CV, and blog/RSS structure where possible.
- Hide Blog from v0 navigation but keep blog support if Astrofy includes it.
- Remove or disable Store.
- Use placeholder case studies and PoCs for v0.
- Do not build real backend demos, contact form backend, analytics, CMS, architecture diagrams, or custom design system work in v0.
- Main site should be deployable to Cloudflare Pages and independent from future VPS demo/API uptime.

## Required v0 Routes

- `/`
- `/case-studies`
- `/case-studies/llm-rag-assistant`
- `/case-studies/computer-vision-segmentation`
- `/case-studies/async-ai-inference-backend`
- `/pocs`
- `/pocs/rag-document-assistant`
- `/pocs/computer-vision-segmentation`
- `/pocs/async-ai-inference-api`
- `/about`
- `/contact`
- `/cv`

## Navigation

Main navigation must show only:

- Case Studies
- PoCs
- About
- CV
- Contact

Do not show Blog or Store in v0 navigation.

## Homepage Order

1. Hero
2. What I Build
3. Featured Case Studies
4. PoC / Demo Preview
5. Work With Me
6. Tech Stack
7. Availability
8. Contact CTA

## Positioning Copy

Main positioning:

Remote AI/ML Engineer for production AI systems

Supporting copy:

I help teams build LLM/RAG apps, computer vision pipelines, FastAPI model APIs, vector search systems, n8n automations, and cloud inference backends.

Availability:

Based in Indonesia, UTC+7. Available for APAC/Europe overlap and async global teams.

Work type:

Open to remote roles, contractor work, freelance projects, part-time engagements, and project-based AI/backend implementation.

## Current Next Steps

1. Bootstrap Astrofy into this repo.
2. Install dependencies and confirm a baseline build.
3. Audit Astrofy's routes, layouts, navigation, content collections, and metadata conventions.
4. Implement global configuration and v0 navigation.
5. Build pages according to `IMPLEMENTATION_PLAN.md` and `DESIGN.md`.

## Verification Commands

Commands are pending until Astrofy is installed. Expected future commands are likely:

- `npm install`
- `npm run dev`
- `npm run build`

Update this section after package scripts are known.

## Known Blockers / Unknowns

- Actual GitHub URL is not confirmed in repo files yet.
- Actual LinkedIn URL is not confirmed in repo files yet.
- Contact email is not confirmed in repo files yet.
- Final CV PDF is not available yet; use "CV PDF coming soon" unless provided.

## Handoff Rule

Before ending a substantial implementation session, update this file with:

- What changed.
- What commands were run and whether they passed.
- Any important decisions made.
- Any blockers or unresolved questions.
- The next recommended steps.
