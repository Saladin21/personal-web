# AGENTS.md

## Project Mission

Build v0 of Ahmad Saladin's personal website using Astrofy as the base template. The site should help Ahmad win international remote AI/ML/backend opportunities by answering quickly: "Can Ahmad help us build this AI system?"

## Positioning

Use this positioning consistently:

Remote AI/ML Engineer for production AI systems

Supporting copy:

I help teams build LLM/RAG apps, computer vision pipelines, FastAPI model APIs, vector search systems, n8n automations, and cloud inference backends.

Availability:

Based in Indonesia, UTC+7. Available for APAC/Europe overlap and async global teams.

Work type:

Open to remote roles, contractor work, freelance projects, part-time engagements, and project-based AI/backend implementation.

## v0 Scope

Required routes:

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

Keep blog support in the codebase if Astrofy includes it, but hide Blog from v0 navigation. Remove or disable Store.

## Navigation

Main navigation must show only:

- Case Studies
- PoCs
- About
- CV
- Contact

Do not show Blog or Store in v0 navigation.

## Homepage Order

Build the homepage as a proof-of-work landing page in this order:

1. Hero
2. What I Build
3. Featured Case Studies
4. PoC / Demo Preview
5. Work With Me
6. Tech Stack
7. Availability
8. Contact CTA

## Content Rules

- Use placeholder case studies and PoCs for v0.
- Do not create fake testimonials, fake stats, fake logos, fake employers, fake demos, or broken demo links.
- Contact form backend is out of scope. Prefer clear email/contact CTAs unless a form is explicitly labeled as non-functional.
- CV PDF can be marked "CV PDF coming soon" if no final PDF exists.
- Blog content, real backend demos, architecture diagrams, analytics, CMS, and custom design system work are out of scope for v0.

## Visual Direction

Use Astrofy's visual style as the base and customize toward clean, technical, trustworthy, minimal, fast, readable, professional, light-first, and mobile-friendly.

Avoid flashy animations, heavy gradients, AI hype, pricing tables, store/e-commerce sections, and blog-first layouts.

Use `DESIGN.md` as the reusable design reference for layout rhythm, typography, cards, tags, CTAs, responsive behavior, accessibility, and future page consistency. When adding or changing pages, follow `DESIGN.md` unless the user explicitly updates the design direction.

## Session Handoff

Keep `CONTEXT.md` updated when implementation status, decisions, blockers, routes, commands, dependencies, or next steps change. Future sessions should read `CONTEXT.md`, `AGENTS.md`, `DESIGN.md`, and `IMPLEMENTATION_PLAN.md` before making substantial changes.

## SEO

Add basic metadata to all required v0 pages.

Homepage title:

Ahmad Saladin - Remote AI/ML Engineer

Homepage description:

Remote AI/ML engineer based in Indonesia, building production LLM/RAG apps, computer vision pipelines, FastAPI model APIs, and AI automation workflows.

## Done Criteria

v0 is complete when Astrofy is installed and builds successfully, all required routes exist, navigation works, Blog is hidden, Store is removed or disabled, metadata exists, mobile layout works, GitHub/LinkedIn/email links work, no broken internal links remain, and the site is deployable to Cloudflare Pages.
