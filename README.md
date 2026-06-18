# Ahmad Saladin Personal Website

Astrofy-based v0 personal website for Ahmad Saladin, positioned as a remote AI/ML engineer for production AI systems.

## Commands

- `npm run dev`: start local Astro development server.
- `npm run build`: build the static production site into `dist/`.
- `npm run preview`: preview the production build locally.

No lint or format scripts are currently defined in `package.json`.

## Required Routes

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

## Deployment

Cloudflare Pages settings:

- Build command: `npm run build`
- Output directory: `dist`
- Environment variables: none required for v0

The v0 site is static and does not depend on a VPS, hosted model, queue, webhook, or live demo backend.

## Known Pending Content

- Actual email address
- Actual GitHub URL
- Actual LinkedIn URL
- Final CV PDF

These are marked as pending in the UI rather than using fake or broken links.
