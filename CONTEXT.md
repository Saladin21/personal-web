# Project Context

## Purpose

This file is the handoff note for future coding sessions. Keep it current whenever implementation status, decisions, blockers, commands, dependencies, routes, or next steps change.

## Current State

- Astrofy is installed in this repo and a baseline build passes after removing the incompatible sitemap integration from `astro.config.mjs`.
- Source brief exists in `brief.md`.
- Agent instructions exist in `AGENTS.md`.
- Reusable design guidance exists in `DESIGN.md`.
- Detailed implementation plan exists in `IMPLEMENTATION_PLAN.md`.
- Astrofy source files live under `src/`, static assets under `public/`, and package scripts are in `package.json`.

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
- Implement v0 case studies and PoCs as static Astro pages instead of adding new content collections. This is the smallest safe fit for placeholder pages and keeps the Astrofy blog collection intact for later.

## Astrofy Structure Audit

- Global metadata defaults: `src/config.ts`.
- Astro config and integrations: `astro.config.mjs`.
- Shared page shell: `src/layouts/BaseLayout.astro`.
- Metadata tags: `src/components/BaseHead.astro`.
- Mobile header branding: `src/components/Header.astro`.
- Sidebar navigation: `src/components/SideBarMenu.astro`.
- Sidebar social/contact links: `src/components/SideBarFooter.astro`.
- Footer copyright/template credit: `src/components/Footer.astro`.
- Homepage: `src/pages/index.astro`.
- Existing CV page: `src/pages/cv.astro`.
- Existing project/service template pages: `src/pages/projects.astro` and `src/pages/services.astro`.
- Blog routes: `src/pages/blog/` with content in `src/content/blog/`; keep support but hide from v0 navigation.
- RSS route: `src/pages/rss.xml.js`.
- Store routes: `src/pages/store/` with content in `src/content/store/`; remove or disable for v0.
- Content collection schemas: `src/content/config.ts`.

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

1. Implement global configuration and v0 navigation.
2. Remove or disable Store routes and content from the v0 user journey.
3. Build pages according to `IMPLEMENTATION_PLAN.md` and `DESIGN.md`.

## Verification Commands

- `npm run dev -- --host 127.0.0.1`: starts Astro dev server.
- `npm run build`: passes after disabling the incompatible Astrofy sitemap integration.

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
