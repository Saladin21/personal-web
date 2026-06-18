# Ahmad Saladin Personal Website v0 Build Brief

## Project Goal

Build v0 of Ahmad Saladin’s personal website using Astrofy as the base template.

The goal of v0 is to get the website live with a polished template, working navigation, clear landing page, page structure, and placeholder pages for future case studies and PoCs.

The goal is not to finish all portfolio content yet.

The website should support both:

1. Remote job searching
2. Contractor, freelance, part-time, and project-based AI/backend work

The site should answer this question quickly:

Can Ahmad help us build this AI system?

## Base Template

Use Astrofy as the base template.

Keep Astrofy’s useful strengths:

* Astro + Tailwind structure
* Personal portfolio style
* Project/content structure
* CV support
* Blog/RSS support for later
* Clean technical presentation

Modify Astrofy so it does not feel like a generic personal blog or resume site.

## Main Positioning

Use this positioning throughout the site:

Remote AI/ML Engineer for production AI systems

Supporting copy:

I help teams build LLM/RAG apps, computer vision pipelines, FastAPI model APIs, vector search systems, n8n automations, and cloud inference backends.

Availability:

Based in Indonesia, UTC+7. Available for APAC/Europe overlap and async global teams.

Work type:

Open to remote roles, contractor work, freelance projects, part-time engagements, and project-based AI/backend implementation.

## Audience

The site is for:

* International remote recruiters
* Startup founders
* Technical hiring managers
* AI agencies
* Freelance marketplace clients
* Upwork/Contra/Braintrust clients
* Potential consulting/project clients

The site should work for both:

* Someone hiring Ahmad into a team
* Someone asking Ahmad to build an AI system or PoC

## v0 Scope

Build these pages:

* `/`
* `/case-studies`
* `/case-studies/llm-rag-assistant`
* `/case-studies/computer-vision-segmentation`
* `/case-studies/async-ai-inference-backend`
* `/pocs`
* `/pocs/rag-document-assistant`
* `/pocs/computer-vision-segmentation`
* `/pocs/async-ai-inference-api`
* `/about`
* `/contact`
* `/cv`

Keep `/blog` in the codebase if Astrofy includes it, but hide it from the main navigation in v0.

Remove or disable any Store section.

## Navigation

Main navigation:

* Case Studies
* PoCs
* About
* CV
* Contact

Do not show Blog in the v0 navigation.

Do not show Store.

## Homepage Structure

The homepage should be a proof-of-work landing page.

Use this order:

1. Hero
2. What I Build
3. Featured Case Studies
4. PoC / Demo Preview
5. Work With Me
6. Tech Stack
7. Availability
8. Contact CTA

## Hero Section

Headline:

Remote AI/ML Engineer for production AI systems

Subheadline:

I help teams build LLM/RAG apps, computer vision pipelines, FastAPI model APIs, vector search systems, n8n automations, and cloud inference backends.

Availability line:

Based in Indonesia, UTC+7. Available for APAC/Europe overlap and async global teams.

Work type line:

Open to remote roles, contractor work, freelance projects, part-time engagements, and project-based AI/backend implementation.

Primary CTA:

View Case Studies

Secondary CTAs:

* View PoCs
* View CV
* Contact Me

Secondary links:

* GitHub
* LinkedIn

## What I Build Section

Create four cards.

### 1. LLM/RAG Applications

Description:

Document assistants, retrieval pipelines, vector search, tool-calling workflows, structured data collection, and AI app backends.

Tags:

Python, FastAPI, Qdrant, LangGraph, RAG, Tool Calling

### 2. Computer Vision Systems

Description:

Image processing, segmentation, detection, OpenCV/PyTorch pipelines, sliding-window inference, post-processing, and production inference APIs.

Tags:

PyTorch, OpenCV, ONNX, Segmentation, Detection, Sliding-Window Inference

### 3. AI Backend & Model Serving

Description:

FastAPI/Flask model APIs, async job queues, Redis/RabbitMQ workers, object storage flows, callback/webhook patterns, and cloud deployment.

Tags:

FastAPI, Flask, Redis, RabbitMQ, Docker, AWS, GCP, S3/GCS

### 4. n8n + AI Automation

Description:

Workflow automations combining APIs, LLMs, webhooks, human approval, messaging integrations, and business process automation.

Tags:

n8n, Webhooks, LLMs, Gmail, Telegram, Postgres, Automation

## Featured Case Studies Section

Repurpose Astrofy’s project structure into case studies.

Initial case study cards:

1. LLM/RAG Assistant with Tool Calling
2. Computer Vision Segmentation Pipeline
3. Async AI Inference Backend

Each card should include:

* title
* one-line summary
* tags
* status label: “Case study coming soon”
* link to placeholder detail page

### Case Study Card 1

Title:

LLM/RAG Assistant with Tool Calling

Summary:

AI assistant workflow with retrieval, tool calling, structured information collection, and backend integration.

Tags:

LLM, RAG, Qdrant, FastAPI, LangGraph, Tool Calling

Status:

Case study coming soon

### Case Study Card 2

Title:

Computer Vision Segmentation Pipeline

Summary:

Production-oriented image segmentation workflow with preprocessing, sliding-window inference, post-processing, API/mobile deployment considerations, and visualization outputs.

Tags:

Computer Vision, PyTorch, OpenCV, Segmentation, ONNX, API Deployment

Status:

Case study coming soon

### Case Study Card 3

Title:

Async AI Inference Backend

Summary:

Backend architecture for long-running AI jobs using API endpoints, queue workers, object storage, status tracking, and callback/webhook delivery.

Tags:

FastAPI, Flask, Redis, RabbitMQ, Docker, AWS, GCP, S3/GCS

Status:

Case study coming soon

## Case Study Detail Placeholder Pages

Each case study detail page should exist in v0.

Use this placeholder structure:

# Case Study Title

## Summary

Short paragraph explaining what this case study will cover.

## What This Will Cover

* Problem
* Ahmad’s role
* Solution architecture
* Tech stack
* Key challenges
* Result or practical outcome
* Screenshots/demo assets
* What would be improved next

## Tech Stack

List relevant technologies.

## Status

Full case study coming soon.

## CTA

Interested in building something similar? Contact me.

## PoC Index Page

Create `/pocs`.

This page should explain that PoCs are different from case studies.

Suggested copy:

PoCs are small demos and walkthroughs that show how I would approach common AI system patterns. Some start as guided frontend-only demos with sample data. Real backend demos may later be hosted separately on demo subdomains.

Initial PoC cards:

1. RAG Document Assistant Demo
2. Computer Vision Segmentation Demo
3. Async AI Inference API Demo

Each card should include:

* title
* what it demonstrates
* who it is useful for
* tags
* status label
* link to placeholder detail page

### PoC Card 1

Title:

RAG Document Assistant Demo

What it demonstrates:

A document assistant flow with sample document selection, retrieved context, source-grounded answer, and productionization notes.

Useful for:

Startups, internal teams, and agencies building document Q&A, knowledge base assistants, or retrieval-backed LLM apps.

Tags:

RAG, Vector Search, Qdrant, LLM, FastAPI

Status:

Guided demo planned

### PoC Card 2

Title:

Computer Vision Segmentation Demo

What it demonstrates:

A visual walkthrough of image input, segmentation mask, overlay result, post-processing, and deployment considerations.

Useful for:

Teams building medical, beauty, industrial, or inspection-related image analysis workflows.

Tags:

Computer Vision, OpenCV, PyTorch, Segmentation, ONNX

Status:

Guided demo planned

### PoC Card 3

Title:

Async AI Inference API Demo

What it demonstrates:

A simulated long-running AI inference workflow: submit job, queue, process, store result, check status, and receive callback.

Useful for:

Teams building model-serving APIs, image processing systems, batch inference, or AI backends.

Tags:

FastAPI, Queue, Worker, Redis, RabbitMQ, Storage, Callback

Status:

Guided demo planned

## PoC Detail Placeholder Pages

Each PoC detail page should exist in v0.

Use this structure:

# PoC Title

## What It Does

Short description of the demo.

## Who It Is For

Short list of relevant users.

## Demo Status

For v0, this is a placeholder or static walkthrough.

## Architecture

Simple text flow.

Example:

User → Frontend → API → Queue → Worker → Storage → Status / Callback

## Tech Stack

Relevant tools.

## Limitations

State that the v0 version is not a live backend demo yet.

## Productionization Plan

Mention what would be added for production:

* auth
* monitoring
* retries
* error handling
* rate limits
* evaluation
* scaling
* cost controls

## CTA

Want to build something like this? Contact me.

## Work With Me Section

Add this section to the homepage.

Title:

Available for roles and project work

Description:

I’m available for remote AI/ML engineering roles, contractor engagements, freelance PoCs, part-time implementation support, and project-based AI/backend work.

Create two columns.

### For Hiring Teams

Description:

Looking for an AI/ML engineer who can build production-oriented systems, not just experiments.

Relevant roles:

* AI/ML Engineer
* LLM/RAG Engineer
* Computer Vision Engineer
* AI Backend Engineer
* Python Backend Engineer with ML deployment experience

CTA:

View CV

### For Clients & Agencies

Description:

Need help building AI prototypes, backend integrations, computer vision pipelines, RAG apps, or workflow automations.

Relevant work:

* RAG/document assistant prototypes
* Computer vision pipelines
* Async model inference APIs
* AI workflow automation
* n8n + LLM implementation
* Backend integration for AI products

CTA:

Contact Me

## Tech Stack Section

Show a compact tech stack section.

Group by category.

### AI / ML

* PyTorch
* scikit-learn
* ONNX
* OpenCV
* embeddings
* segmentation
* detection

### LLM / Agents

* RAG
* Qdrant
* LangGraph
* tool calling
* LLM APIs
* prompt workflows

### Backend

* Python
* FastAPI
* Flask
* Redis
* RabbitMQ
* REST APIs
* webhooks

### Cloud / Infra

* Docker
* AWS
* GCP
* S3/GCS
* Cloudflare Pages
* VPS deployment

### Automation

* n8n
* Telegram
* Gmail
* Postgres
* workflow automation

## About Page

Keep the About page short and professional.

Suggested copy:

I’m Ahmad Saladin, an AI/ML engineer based in Indonesia.

I build production-oriented AI systems across LLM apps, computer vision, backend model serving, and workflow automation. My work combines Python backend engineering, ML deployment, and practical AI product development.

I’m available for remote contractor, freelance, part-time, and project-based work with APAC/Europe overlap and async global teams.

Avoid:

* long personal biography
* generic “passionate about AI” wording
* too much focus on being offshore or lower cost
* unrelated personal details

## Contact Page

Create `/contact`.

Include:

* email
* LinkedIn
* GitHub
* location: Indonesia, UTC+7
* availability: APAC/Europe overlap and async global teams
* open to remote jobs, contractor work, freelance projects, part-time engagements, and project-based AI/backend implementation

A contact form can be visually present, but backend functionality can be deferred.

If a form is included in v0, label it clearly if it is not functional yet, or make it a simple mailto/contact CTA instead.

Future form handling options:

* n8n webhook on VPS
* Formspree
* Resend
* Cloudflare Turnstile for spam protection

## CV Page

Create `/cv`.

Include:

* short role summary
* core skills
* selected experience
* links to case studies
* download CV PDF button
* contact CTA

For v0, use one general AI/ML Engineer CV.

If the final PDF is not ready, include a placeholder button or link and mark it as “CV PDF coming soon.”

## Blog Handling

Astrofy may include Blog/RSS support.

Keep blog support in the codebase, but hide blog from the main navigation in v0.

Blog is planned for v2.

Future blog topics should support SEO and credibility, such as:

* Designing async AI inference APIs
* Sliding-window inference for large images
* RAG vs fine-tuning for business apps
* Building reliable LLM tool-calling workflows
* Deploying AI demos without burning GPU/LLM cost

## Demo Strategy

For v0, do not build real backend demos.

Use placeholders and static pages.

For v1, guided frontend-only demos can be added inside Astro pages using sample data.

For real backend demos, use separate subdomains later:

* demo.ahmadsaladin.com
* api.ahmadsaladin.com
* rag-demo.ahmadsaladin.com
* cv-demo.ahmadsaladin.com

The main site should remain independent from VPS uptime.

## Visual Style

Use Astrofy’s default visual style as the base.

Customize toward:

* clean
* technical
* trustworthy
* minimal
* fast
* readable
* professional
* light-first if possible
* mobile-friendly

Avoid:

* overly flashy animations
* heavy gradients
* generic AI hype
* fake testimonials
* fake company logos
* pricing tables
* store/e-commerce sections
* blog-first layout

## SEO / Metadata

Add basic metadata for v0.

Homepage title:

Ahmad Saladin — Remote AI/ML Engineer

Homepage description:

Remote AI/ML engineer based in Indonesia, building production LLM/RAG apps, computer vision pipelines, FastAPI model APIs, and AI automation workflows.

Add metadata to:

* home
* case study index
* each case study placeholder
* PoC index
* each PoC placeholder
* about
* contact
* cv

Blog SEO can wait until v2.

## Deployment

Deploy to Cloudflare Pages.

Main site:

ahmadsaladin.com → Cloudflare Pages

Future demo/API services:

demo.ahmadsaladin.com → VPS

api.ahmadsaladin.com → VPS

The main portfolio website should not depend on VPS uptime.

## v0 Done Criteria

v0 is complete when:

* Astrofy is installed and running
* Store is removed or disabled
* Blog is hidden from v0 navigation
* homepage is rewritten for Ahmad’s AI/ML positioning
* all required routes exist
* case study index exists
* 3 placeholder case study pages exist
* PoC index exists
* 3 placeholder PoC pages exist
* About page exists
* Contact page exists
* CV page exists
* navigation works
* GitHub, LinkedIn, email links work
* layout works on mobile
* basic SEO metadata exists
* site builds successfully
* site deploys to Cloudflare Pages
* no broken internal links
* no fake testimonials, fake stats, fake logos, or broken demo links remain

## Out of Scope for v0

Do not build these yet:

* full case study writing
* final screenshots
* architecture diagrams
* real live demos
* real backend demo APIs
* contact form backend
* n8n webhook integration
* blog content
* role-specific CVs
* analytics
* CMS
* complex animations
* custom design system from scratch

## Final Principle

Do not build a fancy portfolio.

Build a trust-building proof-of-work site that helps Ahmad win international remote AI/ML/backend opportunities.

Optimize for:

* clarity
* credibility
* relevant proof
* fast loading
* easy contact
* reusable case study structure
* future PoCs and blog expansion
