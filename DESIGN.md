# Design Guidelines

## Purpose

Use this document to keep Ahmad Saladin's personal website visually and structurally consistent across v0 pages and future additions.

The site should feel like a clean technical proof-of-work portfolio for a remote AI/ML engineer, not a generic blog, flashy AI landing page, or resume-only site.

## Design Principles

- Clear before clever.
- Technical, trustworthy, minimal, and readable.
- Light-first and fast-loading.
- Proof-of-work focused, with no fake social proof.
- Mobile-friendly by default.
- Reuse Astrofy's existing patterns before inventing new ones.

## Visual Tone

Aim for:

- Calm technical confidence.
- Practical engineering credibility.
- Sparse but not empty.
- Professional enough for recruiters and hiring managers.
- Concrete enough for founders, agencies, and freelance clients.

Avoid:

- Heavy gradients.
- Flashy animations.
- AI hype visuals.
- Fake dashboards or fake metrics.
- Logo walls.
- Testimonial sections.
- Pricing tables.
- Store/e-commerce patterns.

## Page Layout

Use a consistent page rhythm:

- Header navigation.
- Main content container.
- Page hero or intro block.
- Content sections with clear headings.
- Final contact CTA.
- Footer.

Recommended section spacing:

- Use generous vertical spacing between major sections.
- Keep related cards visually grouped.
- Avoid dense resume-like blocks on marketing pages.
- Keep line lengths readable, especially on About, CV, and detail pages.

Recommended page widths:

- Use Astrofy's existing container width where possible.
- Use narrower content width for prose-heavy pages.
- Use wider grids for cards and grouped capabilities.

## Navigation

Main navigation must remain simple:

- Case Studies
- PoCs
- About
- CV
- Contact

Rules:

- Do not show Blog in v0 navigation.
- Do not show Store.
- Keep primary navigation labels short.
- Use the same nav order in desktop and mobile.
- Make Contact easy to find.

## Typography

Use Astrofy's default typography unless there is a strong reason to change it.

Rules:

- Use one clear heading hierarchy per page.
- Use direct, specific headings instead of vague marketing headings.
- Keep paragraphs short.
- Prefer plain technical language over buzzwords.
- Use tags for scannability, not decoration.

Suggested heading style:

- H1: page purpose or main positioning.
- H2: major page sections.
- H3: cards, subsections, and grouped details.

Suggested copy style:

- Concrete: "FastAPI model APIs" instead of "scalable AI innovation".
- Specific: "RAG apps, computer vision pipelines, async inference backends".
- Honest: "Full case study coming soon" where content is placeholder.

## Color and Contrast

Use Astrofy's base palette and keep it restrained.

Rules:

- Prefer light backgrounds.
- Use dark text with strong contrast.
- Use accent color sparingly for links, tags, and primary CTAs.
- Avoid multi-color gradients and overly saturated blocks.
- Make status labels subtle but readable.

Status label examples:

- Case study coming soon
- Guided demo planned
- CV PDF coming soon

## Buttons and Links

Use consistent CTA hierarchy.

Primary CTAs:

- View Case Studies
- Contact Me

Secondary CTAs:

- View PoCs
- View CV
- GitHub
- LinkedIn

Rules:

- Primary buttons should be visually strongest.
- Secondary buttons or links should be clear but quieter.
- Do not link to missing demos, missing PDFs, or incomplete external pages unless clearly labeled.
- Every card link should resolve to a real internal placeholder page.

## Cards

Use cards for capabilities, case studies, PoCs, and grouped CV content.

Card structure:

- Title.
- One concise description.
- Optional metadata or status label.
- Tags.
- One clear link or CTA.

Rules:

- Keep cards similar in density within the same section.
- Do not overload cards with long paragraphs.
- Tags should wrap cleanly on mobile.
- Status labels should set expectations honestly.

## Tags

Use tags to make expertise quickly scannable.

Recommended tag groups:

- Python
- FastAPI
- Flask
- PyTorch
- OpenCV
- ONNX
- RAG
- Qdrant
- LangGraph
- Tool Calling
- Redis
- RabbitMQ
- Docker
- AWS
- GCP
- n8n

Rules:

- Keep tag text short.
- Reuse tag names consistently.
- Do not use tags as fake keyword stuffing.
- Prefer 4 to 7 tags per card.

## Homepage Pattern

The homepage must follow this order:

1. Hero
2. What I Build
3. Featured Case Studies
4. PoC / Demo Preview
5. Work With Me
6. Tech Stack
7. Availability
8. Contact CTA

Hero rules:

- Lead with "Remote AI/ML Engineer for production AI systems".
- Show the supporting copy near the headline.
- Include location and availability early.
- Make CTAs visible without scrolling on desktop where possible.

Section rules:

- What I Build should show capability breadth.
- Featured Case Studies should point to placeholder detail pages.
- PoC / Demo Preview should clearly say demos are planned or static in v0.
- Work With Me should support both hiring teams and project clients.
- Tech Stack should be compact, not a huge skills dump.
- Availability should make timezone and work types obvious.

## Detail Page Pattern

Use detail pages for case studies and PoCs even when content is placeholder.

Case study detail structure:

- H1 case study title.
- Summary.
- What This Will Cover.
- Tech Stack.
- Status.
- CTA.

PoC detail structure:

- H1 PoC title.
- What It Does.
- Who It Is For.
- Demo Status.
- Architecture.
- Tech Stack.
- Limitations.
- Productionization Plan.
- CTA.

Rules:

- Use a consistent intro block on all detail pages.
- Keep placeholder pages honest and useful.
- Include a final contact CTA.
- Do not add fake screenshots, fake architecture diagrams, or fake demo links.

## Contact Pattern

Contact sections and pages should prioritize direct contact.

Include:

- Email.
- LinkedIn.
- GitHub.
- Location: Indonesia, UTC+7.
- Availability: APAC/Europe overlap and async global teams.
- Work types: remote roles, contractor work, freelance projects, part-time engagements, project-based AI/backend implementation.

Rules:

- Prefer mailto/contact links over a fake form.
- If a visual form is added, label it clearly if non-functional.
- Do not imply instant availability or guaranteed response time unless true.

## Responsive Behavior

Mobile requirements:

- No horizontal overflow.
- Navigation remains usable.
- Hero CTAs wrap cleanly.
- Cards stack into one column when needed.
- Tags wrap without breaking layout.
- Long URLs or email addresses do not overflow.

Desktop requirements:

- Use two- or three-column grids where helpful.
- Keep prose width constrained.
- Avoid leaving CTA sections visually disconnected from content.

## Accessibility

Minimum requirements:

- One H1 per page.
- Logical heading order.
- Descriptive link text.
- Good color contrast.
- Keyboard-visible links and buttons.
- Alt text for meaningful images.
- Decorative images should not distract from content.

## Content Integrity

Never add:

- Fake testimonials.
- Fake stats.
- Fake company logos.
- Fake employers.
- Fake live demos.
- Broken demo links.
- Claims that case studies are complete when they are placeholders.

Use honest placeholder language:

- "Case study coming soon"
- "Full case study coming soon"
- "Guided demo planned"
- "This v0 page is not a live backend demo yet"
- "CV PDF coming soon"

## Reusable Section Checklist

Before adding or changing a section, confirm:

- The section supports the main positioning.
- The heading is specific and scannable.
- The copy is concrete and not hype-driven.
- CTAs link to existing pages.
- The design matches existing spacing, cards, tags, and buttons.
- The layout works on mobile.
- No out-of-scope v0 feature is implied.

## Future Expansion

Future additions should preserve the same design language:

- Blog can be added in v2 without becoming the homepage focus.
- Guided frontend-only demos can be added later with sample data.
- Real backend demos should live on separate subdomains.
- New case studies should reuse the same detail page structure before adding custom visuals.
- New PoCs should clearly separate static walkthroughs from live demos.
