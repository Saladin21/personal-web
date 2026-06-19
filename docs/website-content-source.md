# Website Content Source Document

This is the single source of truth for filling in missing/placeholder data on ahmadsaladin.com. Every section maps to a specific page or component on the site.

---

## 1. Contact Links (Homepage + Contact Page)

Replace all placeholder text with these:

- **Email:** ahmadsaladin21@gmail.com
- **LinkedIn:** https://linkedin.com/in/ahmad-saladin/
- **GitHub:** https://github.com/Saladin21
- **Phone:** +62 817625440
- **Kaggle:** https://www.kaggle.com/ahmadsaladin

---

## 2. Hero / Homepage Introduction

### Headline
**Remote AI/ML Engineer for production AI systems**

### Subline (recommended rewrite)
> I build and deploy LLM/RAG applications, computer vision pipelines, FastAPI model APIs, real-time AI workflows, and AI automation systems. Based in Indonesia, UTC+7. Available for APAC/Europe overlap and async global teams.

### Suggested stronger subtitle (replaces the generic "I help teams build...")
> I help teams ship production AI: retrieval pipelines, voice AI, evaluation frameworks, model serving, and end-to-end AI product development.

---

## 3. Case Studies (Homepage + /case-studies)

### Case Study 1: LLM/RAG Assistant with Tool Calling

- **Title:** LLM/RAG Assistant with Tool Calling
- **Status:** Write the full case study (currently placeholder)
- **Tech:** Python, FastAPI, Qdrant, LangChain, LlamaIndex, OpenAI API, tool calling
- **Problem:** Enterprise client needed a document assistant that could retrieve relevant knowledge from ingested PDFs and websites, answer questions with source grounding, and collect structured information via tool calling.
- **Approach:** Built a RAG pipeline using LlamaIndex for document ingestion and retrieval, Qdrant for vector search, and LangChain for orchestration. Implemented tool calling for structured data collection (appointment booking, information intake). Ingested client documents/PDFs and scraped client websites with Playwright for knowledge base population. Designed the system to handle real-time client-facing interactions with reliability and low latency.
- **Key decisions:**
  - Chose Qdrant over FAISS for production-ready vector search with filtering
  - Used Playwright for web scraping to handle JS-rendered client pages
  - Implemented structured output schemas for tool calling to ensure reliable data collection
- **Outcome:** Production system handling customer-facing healthcare workflows where latency, reliability, and maintainability mattered.
- **Role:** Sole engineer on the RAG and tool-calling components.

### Case Study 2: Computer Vision Segmentation Pipeline

- **Title:** Computer Vision Segmentation Pipeline
- **Status:** Write the full case study (currently placeholder)
- **Tech:** Python, Flask, PyTorch, RabbitMQ, AWS, OpenCV, ONNX, TorchScript, JNI
- **Problem:** Healthcare-adjacent client needed automated image segmentation for clinical workflow support, with both cloud API access and offline mobile deployment.
- **Approach:** Built an asynchronous inference pipeline using Flask (API layer), RabbitMQ (job queuing), and PyTorch (model inference). Developed sliding-window inference for large image processing, post-processing for mask refinement, and visualization outputs. Deployed optimized models to Android using TorchScript and JNI for offline inference.
- **Key decisions:**
  - Used async queue architecture to handle variable inference load without blocking
  - TorchScript + JNI for mobile deployment to avoid on-device Python runtime
  - Sliding-window approach to handle images larger than model input resolution
- **Outcome:** Production pipeline serving a healthcare-adjacent workflow with both cloud and mobile deployment paths.
- **Role:** Built and maintained the full pipeline (API, queue, inference, deployment).

### Case Study 3: Async AI Inference Backend

- **Title:** Async AI Inference Backend
- **Status:** Write the full case study (currently placeholder)
- **Tech:** Python, FastAPI, Flask, Redis, RabbitMQ, Docker, AWS, GCP, S3/GCS, webhooks
- **Problem:** Client needed a backend architecture for long-running AI jobs that could accept API requests, queue work for background processing, store results, track status, and deliver results via callbacks/webhooks.
- **Approach:** Designed an async job processing architecture with FastAPI endpoints for job submission, RabbitMQ/Redis for queuing, worker processes for inference, object storage (S3/GCS) for result persistence, and webhook callbacks for result delivery. Implemented status tracking and error handling throughout the pipeline.
- **Key decisions:**
  - Decoupled submission from processing via queue for scalability
  - Object storage for results to avoid database bloat from large inference outputs
  - Webhook callbacks for real-time result delivery to integrating systems
- **Outcome:** Reusable async inference pattern deployed across multiple AI projects at Infidea.
- **Role:** Designed and built the full architecture.

---

## 4. PoC / Demo Pages (Homepage + /pocs)

### PoC 1: RAG Document Assistant Demo
- **Title:** RAG Document Assistant Demo
- **Status:** Build a guided demo page
- **Description:** A document assistant flow with sample document selection, retrieved context, source-grounded answer generation, and productionization notes.
- **Tech badges:** RAG, Vector Search, Qdrant, LLM, FastAPI
- **Demo flow (suggested):**
  1. User selects a sample document (PDF or web page)
  2. Document is chunked and embedded into Qdrant
  3. User asks a question
  4. System retrieves relevant chunks and generates a source-grounded answer
  5. Display answer with source citations
- **Productionization notes to include:**
  - Chunking strategy choices (size, overlap, metadata)
  - Embedding model selection tradeoffs
  - Qdrant vs FAISS vs managed vector DB
  - Authentication, rate limiting, error handling for production

### PoC 2: Computer Vision Segmentation Demo
- **Title:** Computer Vision Segmentation Demo
- **Status:** Build a guided demo page
- **Description:** A visual walkthrough of image input, segmentation mask generation, overlay result, post-processing, and deployment considerations.
- **Tech badges:** Computer Vision, OpenCV, PyTorch, Segmentation, ONNX
- **Demo flow (suggested):**
  1. Upload or select a sample image
  2. Run segmentation model (browser-based or API)
  3. Display original image, predicted mask, and overlay
  4. Show post-processing steps (morphological operations, contour extraction)
  5. Deployment considerations (ONNX export, mobile optimization, API design)

### PoC 3: Async AI Inference API Demo
- **Title:** Async AI Inference API Demo
- **Status:** Build a guided demo page
- **Description:** A simulated long-running AI inference workflow: submit job, queue, process, store result, check status, and receive callback.
- **Tech badges:** FastAPI, Queue, Worker, Redis, RabbitMQ, Storage, Callback
- **Demo flow (suggested):**
  1. Submit a job via API form (upload input or provide parameters)
  2. Job enters queue, status changes to "processing"
  3. Worker processes the job (simulated or real inference)
  4. Result stored, status changes to "completed"
  5. User checks status endpoint or receives webhook callback
  6. Display result with timing information

---

## 5. About Page (/about)

The current About page is thin. Here is recommended content:

### About Ahmad Saladin

I am Ahmad Saladin, an AI/ML engineer and CEO of Infidea, based in Jakarta, Indonesia. I build production-oriented AI systems across LLM applications, computer vision, backend model serving, and workflow automation.

**What I focus on:**
- LLM/RAG applications with retrieval, vector search, and tool calling
- Computer vision pipelines for segmentation, detection, and image processing
- FastAPI/Flask model APIs and async inference backends
- Real-time AI workflows (voice AI, telephony, LiveKit)
- n8n and AI automation workflows for business processes

**Background:**
- MS Computer Science, University of Colorado Boulder (2025-2026, expected)
- BS Informatics, Institut Teknologi Bandung (GPA: 3.87/4.00)
- Kaggle Competition Expert (Rank 3215 / 200,000, top 1.6%)
- 3+ years building production ML systems, LLM applications, computer vision, and cloud inference pipelines

**What drives my work:**
I care about building AI systems that actually ship and stay reliable in production, not just demos that work in notebooks. My work combines Python backend engineering, ML deployment, and practical AI product development. I've built systems for healthcare workflows, enterprise knowledge management, and real-time AI interactions.

I am available for remote roles, contractor work, freelance projects, part-time engagements, and project-based AI/backend implementation with APAC/Europe overlap and async global teams.

---

## 6. CV Page (/cv)

### Full CV Content

**Name:** Ahmad Saladin
**Role:** Remote AI/ML Engineer for production AI systems
**Location:** Jakarta, Indonesia, UTC+7

---

#### Summary
AI engineer and CEO with 3+ years of experience across production ML systems, LLM applications, computer vision, and cloud inference pipelines. Builds end-to-end AI systems from frontend to backend to AI/ML integration. Strong in workflow design, structured outputs, evaluation criteria, and AI-assisted implementation.

---

#### Experience

**AI Engineer | Infidea | July 2024 -- Present | Jakarta, Indonesia**
- Designed and built real-time patient intake and coordination workflow for an aesthetic clinic using LiveKit, GPT-Realtime, LangChain, and OpenAI API
- Built RAG system using LlamaIndex and Qdrant vector store for knowledge base, ingesting client documents/PDFs and scraping websites with Playwright
- Designed, built, and managed FastAPI services for agentic applications, integrating with Calendly and Google Calendar for appointment booking
- Built AI receptionist with Twilio and LiveKit for voice-based interactions with backend API integration
- Built AI video short generation system using Gemini video understanding + FFmpeg for content analysis and editing

**Data Scientist | Infidea | July 2023 -- June 2024 | Jakarta, Indonesia**
- Built and maintained asynchronous computer vision inference pipeline using Flask, RabbitMQ, PyTorch, and AWS
- Developed image segmentation systems for healthcare-adjacent workflows
- Deployed optimized PyTorch models to Android using TorchScript and JNI for offline inference

**Data Scientist Intern | PT Telkom Indonesia | Aug. 2022 -- Dec. 2022 | Jakarta, Indonesia**
- Built image classification and segmentation models for applied ML use cases
- Conducted hyperparameter tuning with Optuna

**Tenaga Ahli (Informatics) | Lapi Ganesha Utama | 2026 -- Present | Bandung, Indonesia**
- Part of a consulting team for water resource management project (Perum Jasa Tirta II, state-owned enterprise)
- Informatics expertise within government Grand Design project

---

#### Projects

**LLM Fortify | Python, LangChain, Ragas | 2024**
Web app for evaluating OpenAI-compatible LLM endpoints. Adversarial testing, robustness evaluation, modular multi-LLM judging workflow, failure-mode assessment.

**RAG Knowledge Base | Python, FastAPI, LlamaIndex, Qdrant, Playwright | 2026**
RAG system for enterprise knowledge base. Document/PDF ingestion, website scraping with Playwright, vector search with Qdrant, source-grounded answer generation.

**AI Receptionist | Python, FastAPI, Twilio, LiveKit, LangChain, OpenAI API | 2026**
Voice-based AI receptionist for healthcare clinic. Telephony integration via Twilio, real-time voice via LiveKit, backend API for appointment booking.

**Multi-index Query on Image Database | Python, Streamlit, FAISS | 2023**
Semantic retrieval system with SQL-like multi-index queries over image data. CLIP + YOLO integration for structured querying over unstructured inputs.

**Client Inference | JavaScript, Transformers.js | 2025**
Browser-based ML inference demo running NLP and computer vision models fully client-side. Edge/client inference and deployment tradeoff exploration.

**Voice of Customer Pipeline | Python, topic modeling, sentiment analysis | 2026**
Data pipeline for voice of customer analysis. Scraped social media posts enriched with topic modeling and sentiment analysis for customer insights.

---

#### Education

**University of Colorado Boulder** | Boulder, CO
Master of Science in Computer Science | Jan. 2025 -- Dec. 2026 (Expected)

**Institut Teknologi Bandung** | Bandung, Indonesia
Bachelor of Science in Informatics/Computer Science | Aug. 2019 -- Sep. 2023
GPA: 3.87 / 4.00

---

#### Technical Skills

**AI / ML:** PyTorch, scikit-learn, ONNX, OpenCV, embeddings, segmentation, detection, LangChain, LlamaIndex, RAG, Qdrant, FAISS, OpenAI API, Gemini API, GPT-Realtime, LangGraph, tool calling

**Backend:** Python, FastAPI, Flask, Redis, RabbitMQ, REST APIs, webhooks, async pipelines

**Languages:** Python, JavaScript/TypeScript, SQL, Kotlin, C/C++

**Cloud / Infra:** Docker, AWS, GCP, S3/GCS, Cloudflare Pages, VPS deployment

**Automation:** n8n, Telegram Bot API, Gmail API, Postgres, workflow automation

---

#### Certifications & Achievements

**Kaggle Competition Expert** -- Rank 3215 / 200,000 (top 1.6%)

---

## 7. Social / OG Image

- **Current file:** social_img.webp (exists, WebP format)
- **Recommended:** Update with a professional headshot or branded graphic that includes "Ahmad Saladin | AI/ML Engineer" text overlay
- **Dimensions:** Should be 1200x630px for optimal social sharing

---

## 8. Homepage "What I Build" Cards

These are mostly complete. Optional improvement — add metrics or scope where truthful:

### LLM/RAG Applications
- Current: "Document assistants, retrieval pipelines, vector search, tool-calling workflows, structured data collection, and AI app backends."
- **Suggested addition:** "Built for enterprise clients in healthcare and business automation."

### Computer Vision Systems
- Current: "Image processing, segmentation, detection, OpenCV/PyTorch pipelines, sliding-window inference, post-processing, and production inference APIs."
- **Suggested addition:** "Deployed to both cloud APIs and mobile devices (TorchScript + JNI)."

### AI Backend & Model Serving
- Current: "FastAPI/Flask model APIs, async job queues, Redis/RabbitMQ workers, object storage flows, callback/webhook patterns, and cloud deployment."
- **Suggested addition:** "Serving real-time healthcare workflows and long-running inference jobs."

### n8n + AI Automation
- Current: "Workflow automations combining APIs, LLMs, webhooks, human approval, messaging integrations, and business process automation."
- **Suggested addition:** "Built for business process automation with LLM integration."

---

## 9. Tech Stack Section (Homepage)

### Recommended updates based on actual experience:

**AI / ML:** PyTorch, scikit-learn, ONNX, OpenCV, embeddings, segmentation, detection, LangChain, LlamaIndex
**LLM / Agents:** RAG, Qdrant, FAISS, LangGraph, tool calling, OpenAI API, Gemini API, GPT-Realtime, prompt workflows
**Backend:** Python, FastAPI, Flask, Redis, RabbitMQ, REST APIs, webhooks, async pipelines
**Cloud / Infra:** Docker, AWS, GCP, S3/GCS, Cloudflare Pages, VPS deployment
**Automation:** n8n, Telegram, Gmail, Postgres, workflow automation
**Languages:** Python, JavaScript/TypeScript, SQL, Kotlin, C/C++

---

## 10. Footer Content

- **Current:** "Remote AI/ML Engineer for production AI systems."
- **Suggested:** Keep current, but add social links once ready:
  - GitHub: https://github.com/Saladin21
  - LinkedIn: https://linkedin.com/in/ahmad-saladin/
  - Kaggle: https://www.kaggle.com/ahmadsaladin
  - Email: ahmadsaladin21@gmail.com

---

## 11. SEO / Meta Tags

Current meta tags are good. No changes needed. Existing OG image (social_img.webp) is functional.

---

## 12. Missing Data Priority Checklist

### Critical (before public launch):
- [ ] Wire up GitHub link (https://github.com/Saladin21)
- [ ] Wire up LinkedIn link (https://linkedin.com/in/ahmad-saladin/)
- [ ] Wire up email (ahmadsaladin21@gmail.com)
- [ ] Remove all "coming soon" / "pending" placeholder text

### High priority (first week):
- [ ] Write Case Study 1 (LLM/RAG Assistant) — use content from Section 3 above
- [ ] Write Case Study 2 (CV Segmentation) — use content from Section 3 above
- [ ] Write Case Study 3 (Async Inference Backend) — use content from Section 3 above
- [ ] Flesh out About page — use content from Section 5 above
- [ ] Fill in CV page with full experience — use content from Section 6 above

### Medium priority (first month):
- [ ] Build PoC demo pages — use flows from Section 4 above
- [ ] Add Kaggle badge/link prominently (top 1.6% is a differentiator)
- [ ] Update hero subtitle to be more impact-focused
- [ ] Update social/OG image with branded graphic

### Nice to have:
- [ ] Add 2-3 blog posts or insights (RAG tips, CV deployment lessons)
- [ ] Add testimonials or client quotes (if available)
- [ ] Add a "Uses" or "Tools I Use" page for developer audience
