# Implementation Plan

## Goal

Build v0 of Ahmad Saladin's personal website from Astrofy, focused on a polished proof-of-work landing page, complete route structure, placeholder case studies and PoCs, basic SEO, and Cloudflare Pages readiness.

## Principles

- Start from Astrofy instead of building a custom design system.
- Ship a complete, trustworthy v0 before adding real demos or full portfolio content.
- Optimize for clarity, credibility, fast loading, easy contact, and future expansion.
- Keep the main site static and independent from future VPS demo/API uptime.
- Prefer static placeholders over non-functional interactive demos.

## Phase 1: Bootstrap Astrofy

### Tasks

- Install or import Astrofy as the base Astro project.
- Confirm the project uses Astro, Tailwind, content/project structures, CV support, and blog/RSS support where available.
- Install dependencies.
- Run the development server locally.
- Run an initial production build to establish a clean baseline.

### Deliverables

- Working Astrofy-based project in this repo.
- Package scripts for development and build.
- Baseline build passes before content customization begins.

### Verification

- `npm install` or equivalent package manager command succeeds.
- `npm run dev` starts locally.
- `npm run build` succeeds.

## Phase 2: Audit Template Structure

### Tasks

- Identify Astrofy's page, layout, component, navigation, content, and config files.
- Locate any existing Blog, Store, Project, CV, and metadata handling.
- Determine the smallest safe set of files to modify for v0.
- Preserve useful Astrofy conventions instead of rewriting structure unnecessarily.

### Deliverables

- Clear mapping of where pages, navigation, data, and layout are defined.
- Decision on whether case studies and PoCs should use content collections, static Astro pages, or existing project structures.

### Verification

- Required implementation locations are known before broad edits begin.
- No template feature is removed unless it conflicts with v0 scope.

## Phase 3: Global Configuration and Navigation

### Tasks

- Update site identity to Ahmad Saladin.
- Configure global metadata defaults.
- Update navigation to show only Case Studies, PoCs, About, CV, and Contact.
- Hide Blog from main navigation while keeping blog/RSS support in the codebase if present.
- Remove or disable Store routes, navigation, data, and CTAs if Astrofy includes Store functionality.
- Add or update GitHub, LinkedIn, and email links once actual URLs are known.

### Deliverables

- Correct global site name and metadata baseline.
- v0 navigation matches scope.
- No Store UI remains reachable from the primary user journey.

### Verification

- Header and footer navigation contain no Blog or Store links.
- Internal navigation links resolve to existing routes.
- Social/contact links are not placeholders unless explicitly marked.

## Phase 4: Homepage Rewrite

### Tasks

- Rewrite `/` as a proof-of-work landing page.
- Implement the Hero section with the required headline, subheadline, availability line, work type line, primary CTA, secondary CTAs, and GitHub/LinkedIn links.
- Add What I Build with four cards: LLM/RAG Applications, Computer Vision Systems, AI Backend & Model Serving, and n8n + AI Automation.
- Add Featured Case Studies with three placeholder cards and links to detail pages.
- Add PoC / Demo Preview with three placeholder demo cards and links to PoC detail pages.
- Add Work With Me with two columns: For Hiring Teams and For Clients & Agencies.
- Add compact Tech Stack grouped by AI/ML, LLM/Agents, Backend, Cloud/Infra, and Automation.
- Add Availability and Contact CTA sections.
- Keep layout responsive and aligned with Astrofy's visual style.

### Deliverables

- Complete v0 homepage with all required sections in the specified order.
- CTAs route to `/case-studies`, `/pocs`, `/cv`, and `/contact`.

### Verification

- Homepage content matches the positioning in `brief.md`.
- No fake claims, testimonials, logos, metrics, or live demo promises are introduced.
- Mobile and desktop layouts are readable.

## Phase 5: Case Study Pages

### Tasks

- Create `/case-studies` index page.
- Add three case study cards: LLM/RAG Assistant with Tool Calling, Computer Vision Segmentation Pipeline, and Async AI Inference Backend.
- Create detail placeholder pages for each case study.
- Use the required detail structure: Summary, What This Will Cover, Tech Stack, Status, and CTA.
- Add relevant metadata to index and detail pages.

### Deliverables

- `/case-studies`
- `/case-studies/llm-rag-assistant`
- `/case-studies/computer-vision-segmentation`
- `/case-studies/async-ai-inference-backend`

### Verification

- Each case study card links to an existing detail page.
- Each detail page clearly says the full case study is coming soon.
- CTA points users to contact Ahmad without implying a live demo exists.

## Phase 6: PoC Pages

### Tasks

- Create `/pocs` index page.
- Explain that PoCs are small demos and walkthroughs, distinct from case studies.
- Add three PoC cards: RAG Document Assistant Demo, Computer Vision Segmentation Demo, and Async AI Inference API Demo.
- Create detail placeholder pages for each PoC.
- Use the required detail structure: What It Does, Who It Is For, Demo Status, Architecture, Tech Stack, Limitations, Productionization Plan, and CTA.
- State clearly that v0 PoCs are placeholders or static walkthroughs, not live backend demos.

### Deliverables

- `/pocs`
- `/pocs/rag-document-assistant`
- `/pocs/computer-vision-segmentation`
- `/pocs/async-ai-inference-api`

### Verification

- Each PoC card links to an existing detail page.
- No page depends on a live VPS, API, hosted model, webhook, or demo backend.
- Limitations are explicit.

## Phase 7: About, Contact, and CV

### Tasks

- Create or rewrite `/about` with short professional copy.
- Create `/contact` with email, LinkedIn, GitHub, Indonesia UTC+7 location, availability, and work types.
- Avoid a backend contact form for v0 unless it is explicitly labeled as non-functional.
- Create `/cv` with role summary, core skills, selected experience, links to case studies, CV PDF button or "CV PDF coming soon" state, and contact CTA.
- Add metadata to all three pages.

### Deliverables

- `/about`
- `/contact`
- `/cv`

### Verification

- About page avoids long biography and generic AI passion wording.
- Contact page provides a clear way to reach Ahmad.
- CV page does not link to a missing PDF unless clearly marked as coming soon.

## Phase 8: SEO, Accessibility, and Link Integrity

### Tasks

- Add page-specific titles and descriptions for all required routes.
- Confirm semantic heading order on key pages.
- Confirm internal links, CTAs, and footer links resolve.
- Confirm images, icons, and decorative elements do not create accessibility issues.
- Remove or replace any leftover template content that conflicts with v0 positioning.

### Deliverables

- Basic metadata on every v0 page.
- No obvious broken internal links.
- No misleading template content remains.

### Verification

- Build output contains all required routes.
- Manual navigation through all routes succeeds.
- Search for Blog/Store references confirms they are absent from v0 navigation.

## Phase 9: Responsive Polish

### Tasks

- Review homepage, case study pages, PoC pages, About, Contact, and CV on mobile and desktop breakpoints.
- Adjust spacing, card grids, line length, and CTA wrapping.
- Keep styling light, clean, fast, technical, and professional.
- Avoid heavy animations and large visual assets.

### Deliverables

- Mobile-friendly v0 layout.
- Consistent visual language across pages.

### Verification

- No horizontal overflow on mobile.
- CTAs remain visible and usable.
- Cards and tag lists wrap cleanly.

## Phase 10: Build and Deployment Readiness

### Tasks

- Run formatting/linting commands available in the project.
- Run the production build.
- Fix any build, routing, or type errors.
- Confirm Cloudflare Pages build settings, usually `npm run build` and output directory `dist` for Astro.
- Document any required environment variables. v0 should not require demo/API secrets.

### Deliverables

- Production-ready static site build.
- Cloudflare Pages deployment notes if needed.

### Verification

- `npm run build` succeeds.
- No required route is missing from the production build.
- No v0 feature depends on VPS uptime.

## Required Content Inventory

### Case Studies

- LLM/RAG Assistant with Tool Calling: AI assistant workflow with retrieval, tool calling, structured information collection, and backend integration.
- Computer Vision Segmentation Pipeline: Production-oriented image segmentation workflow with preprocessing, sliding-window inference, post-processing, API/mobile deployment considerations, and visualization outputs.
- Async AI Inference Backend: Backend architecture for long-running AI jobs using API endpoints, queue workers, object storage, status tracking, and callback/webhook delivery.

### PoCs

- RAG Document Assistant Demo: sample document selection, retrieved context, source-grounded answer, and productionization notes.
- Computer Vision Segmentation Demo: image input, segmentation mask, overlay result, post-processing, and deployment considerations.
- Async AI Inference API Demo: submit job, queue, process, store result, check status, and receive callback.

### Tech Stack Groups

- AI / ML: PyTorch, scikit-learn, ONNX, OpenCV, embeddings, segmentation, detection.
- LLM / Agents: RAG, Qdrant, LangGraph, tool calling, LLM APIs, prompt workflows.
- Backend: Python, FastAPI, Flask, Redis, RabbitMQ, REST APIs, webhooks.
- Cloud / Infra: Docker, AWS, GCP, S3/GCS, Cloudflare Pages, VPS deployment.
- Automation: n8n, Telegram, Gmail, Postgres, workflow automation.

## Final Acceptance Checklist

- Astrofy is installed and running.
- Store is removed or disabled.
- Blog is hidden from v0 navigation.
- Homepage is rewritten for Ahmad's AI/ML positioning.
- All required routes exist.
- Case study index exists.
- Three placeholder case study pages exist.
- PoC index exists.
- Three placeholder PoC pages exist.
- About page exists.
- Contact page exists.
- CV page exists.
- Navigation works.
- GitHub, LinkedIn, and email links work or are clearly marked if still pending.
- Layout works on mobile.
- Basic SEO metadata exists.
- Site builds successfully.
- Site is ready for Cloudflare Pages deployment.
- No broken internal links remain.
- No fake testimonials, fake stats, fake logos, or broken demo links remain.
