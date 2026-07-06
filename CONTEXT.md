# CONTEXT

Merged reference file combining all documents in this repository into one place. Each section below corresponds to one original file, in the same order as the folder structure.

---

# FILE: README.md

## My AI Journey

Personal knowledge base documenting my path into AI Automation and Agentic AI, built by Lilia Avagyan.

### Background

I come from a tourism and customer experience background and am transitioning into Travel Tech + AI, combining that domain knowledge with automation and agentic AI skills.

### The Path

On April 15, 2026, I started the AI Automation / Agentic AI track of the AGBU Women Coders Program at ARDY Academy in Yerevan, taught by Varazdat Avetisyan, PhD, and coordinated by Gayane Abgaryan. The program ran 32 hours over ten weeks and focused on building real, working AI-powered applications using no-code and low-code tools alongside traditional development.

Over the course, I completed 19 hands-on mini-projects across a wide range of platforms: Opal, Lovable, Bolt.new, Vercel, Create.xyz, Replit, Make.com, Google Apps Script, Hugging Face, Cloudflare, and others. Each project was a chance to test a different tool against a real use case, from AI travel guides to Telegram bots to resume analyzers.

On June 24, 2026, I graduated with distinction, presenting three final projects (an AI-powered job board automation, a full-stack portfolio site, and a TravelTech insights dashboard with an AI chatbot) to roughly 20 students and the AGBU organizers.

After graduation, I enrolled in an advanced follow-up course and set up a fully isolated training environment (new email, new GitHub organization, new Neon and Replit instances) to run a complete mock client delivery: a tourism booking system, built and handed over exactly as I would for a real client.

This repository is where I am consolidating that journey.

### What's Here

- **01-course-projects.md**: table of all 19 hands-on mini-projects from the course, with tools, stacks, and live links.
- **02-agbu-final-projects/**: detailed write-ups of the three AGBU final projects: job board automation, portfolio website, and TravelTech insights.
- **03-client-work/**: the tourism booking system training exercise, a full mock client delivery simulation.
- **04-skills-matrix.md**: summary of tools and skills across all projects.
- **05-timeline.md**: chronological view of the whole journey.

### Numbers

- 19 course mini-projects
- 3 AGBU final projects
- 1 full mock client delivery (training exercise)
- 23 projects total

### Skills Summary

No-code and low-code app building (Opal, Lovable, Bolt.new, Vercel, Create.xyz, Replit, Gamma); automation and orchestration (Make.com, n8n, Google Apps Script); LLM integration (OpenAI, Anthropic, Google Gemini, Groq/Llama); agentic web workflows (Manus AI, Comet agentic browser); full-stack development (Next.js, React, TypeScript, Python/FastAPI); databases (PostgreSQL via Supabase and Neon, Airtable, Google Sheets); chatbots and conversational interfaces (Telegram Bot API, Typebot, Botpress); analytics and admin dashboards; and secure handover practices (row-level security, environment secrets, credential rotation checklists).

Currently enrolled in an advanced agentic AI course, continuing to build toward a Travel Tech + AI specialization.

---

# FILE: 01-course-projects.md

## Course Projects

19 hands-on mini-projects completed during the AI Automation / Agentic AI track at AGBU Women Coders Program, ARDY Academy, Yerevan (April 15 – June 17, 2026). Each project was built to test a specific no-code, low-code, or agentic tool against a real use case.

| # | Project | Live URL | Tool | Tech Stack | Description |
|---|---|---|---|---|---|
| 1 | Beth Hart Live Experience | https://opal.google/app/1c2qEySDrbyJbRQnGT8e4dEhP2AfGsqsN | Opal (Google) | Opal blocks, LLM content generation | AI tour landing page for the nearest Beth Hart concert. Based on date, budget, and days, picks the concert city and generates a page with flights, hotel, expenses, and visa requirements. |
| 2 | Explorer Syunik | https://opal.google/app/16I2YeOrrBFyHVmWGaknn1uxkBjyUFIIk | Opal (Google) | Opal, Maps/embed widgets | AI guide to the Syunik region: key sights, routes, and descriptions generated in Opal. |
| 3 | Homework AI Tracker | https://opal.google/app/1Z5NY8VBZjAMRROPMmbPpLHr-bjpyFAhd | Opal (Google) | Opal, task tracking templates | Looks up a student by name in a Google Sheets homework tracker and shows their assignments. |
| 4 | Syunik Cinematic Travel Guide | https://syunik-magic-guide.lovable.app/ | Lovable | React, Framer Motion | One-page storytelling guide to Syunik with location cards, photos, facts, and an embedded Armenian duduk music button. Code on GitHub. |
| 5 | Curated Hiking Trails in Armenia | https://wander-armenia-trails.lovable.app/ | Lovable | TypeScript, React, Leaflet | Hiking trail catalog for Armenia with region and difficulty filters, plus an embedded Google Map. Code on GitHub. |
| 6 | Vayots Dzor: the Ancient Wine Cradle | https://vayots-dzor-wine-tou-u3c4.bolt.host/ | Bolt.new | React, Tailwind CSS | Landing page about the Vayots Dzor wine region covering history, key wineries, and tastings, with a responsive UI. Code on GitHub. |
| 7 | Yerevan Secrets | https://v0-yerevan-secrets-app.vercel.app/ | Vercel | Next.js, Shadcn UI | Storytelling web app about hidden spots in Yerevan. Code on GitHub. |
| 8 | Armenian Music Box | https://armenian-music-box.created.app/ | Create.xyz | Web Audio API, React | Mini-guide to Armenian musical instruments with a simple audio player. Code on GitHub. |
| 9 | Armenian Stone Alphabet | https://stone-alphabet-sounds--labeautyfl8.replit.app/ | Replit | TypeScript, 3D CSS | Interactive alphabet with voiced Armenian letters, using audio sourced from Wikimedia. Code on GitHub. |
| 10 | The Budget Planner | https://budget-planner-buddy.replit.app/ | Replit | TypeScript, React | Takes a country, city, number of days, and budget, then allocates spending and opens the route in Google Maps. |
| 11 | Website for a New Tour Agency | https://gamma.app/docs/-1f5w9zfvuj4el0o?mode=doc | Gamma | Gamma AI slide-to-site | One-page tour agency site generated directly from an AI presentation in Gamma. |
| 12 | YouTube Researcher Agent | Internal Google Sheet (not public) | Google Apps Script, RapidAPI | Google Sheets, Apps Script, RapidAPI YouTube Search | Agent built inside Google Sheets: a script reads settings, calls the RapidAPI YouTube Search endpoint, and writes results back to the sheet. |
| 13 | AI Advice Visualizer | https://huggingface.co/spaces/liliaavagyan/ai-agents-learning-demo | Hugging Face | Static HTML, CSS, JS | Gives AI-generated advice with a progress visualization; demo mode enabled for safety. |
| 14 | Agentic Browser Scenario (Visa Helper) | Internal Google Doc (not public) | Comet | Agentic browser, Google Docs | Visa Helper scenario built for a tour operator: an agentic browser workflow that finds visa requirements, documents, and deadlines directly from official sites. |
| 15 | Telegram AI Assistant (Lead Capture & Automation) | Telegram: @my_first_agentic_bot | Make.com | Make.com, Telegram Bot API, Google Sheets API, LLM (OpenAI/Anthropic), webhooks | Telegram bot that takes a request, looks up the user in Google Sheets, and passes the data to an LLM to generate the reply. Code on GitHub. |
| 16 | Portfolio-Backend | https://portfolio-backend.replit.app/ | Replit | TypeScript, React, CSS | Early portfolio version showcasing AI Automation, Agentic AI, and full-stack projects. |
| 17 | AI Resume Analyzer | https://resume-analyzer-ai-wg6h.onrender.com | Render | Python, FastAPI, Gemini API | AI-powered resume analyzer built with FastAPI and the Google Gemini API. |
| 18 | AI Portfolio Projects | https://liliaai-8ihxducm.manus.space | Manus AI | React, TypeScript, Tailwind CSS 4, Node.js, MySQL | Professional portfolio site showcasing AI and automation projects from the course. |
| 19 | Lost & Found Hub | https://lost-found-hub.labeautyfl8.workers.dev/ | Cloudflare, Botpress | Python, JS, CSS, HTML, Botpress chatbot | Lost and found platform with item reports, an admin dashboard, and a chatbot. |

Two entries (#12 and #14) link to internal Google Sheets/Docs rather than public pages, so no public URL is listed for those.

---

# FILE: 02-agbu-final-projects/job-board-automation.md

## AI-Powered Job Board Automation

AGBU final project 1. Program: AI Automation / Agentic AI, AGBU Women Coders Program, ARDY Academy, Yerevan. Graduated with distinction, June 24, 2026.

### Goal

Automated pipeline that finds Junior and Entry-level AI Automation and Agentic AI job postings, triggered by a single Telegram button, and returns only results posted in the last 24 hours.

### Tech Stack and Why

- **Manus AI**: autonomous web agent. Used to perform Google Dorking (X-Ray search), which makes LinkedIn's closed job pages reachable through Google's public index. This is a legal search method, not scraping, and Manus provides a visual reasoning log showing its full thought process.
- **Make.com**: orchestration layer, split into two scenarios to support an async architecture: Manus_Job_Launcher and Manus_Data_Receiver.
- **Google Sheets**: results hub, chosen for its native Make.com integration. Two sheets are used: Global Remote (LinkedIn worldwide) and Armenia Local (LinkedIn Armenia, Staff.am, and Job.am).
- **Telegram Bot**: the trigger is a single /search command button rather than free text input, which keeps the interaction simple and saves Make.com operation credits.

### Architecture

The pipeline is split into two independent Make.com scenarios rather than one, because a single scenario hit Make.com's 40-60 second timeout window while the agent was still thinking.

- **Scenario 1: Manus_Job_Launcher:** Telegram (Watch Updates) → filter for the /search command → HTTP POST to the Manus API's task.create endpoint, including a webhook_url for the callback.
- **Scenario 2: Manus_Data_Receiver:** waits on the webhook. Once Manus finishes its search, it posts the results to that webhook. A Router splits the flow into global_remote and armenia_local branches. An Iterator opens the results array, and Google Sheets "Add a Row" writes each vacancy.

This is a push model: the Launcher fires the request and releases immediately rather than waiting for a reply. Manus contacts the Receiver on its own when the results are ready. Full flow: Telegram → Launcher → Manus AI → Receiver → Google Sheets.

### Key Engineering Decisions

- **Hard filters live in the Manus system prompt**, not downstream in Make.com. Manus owns all data-cleanliness responsibility: it rejects Senior/Mid-level roles, postings requiring an EU/US work permit, and anything older than 24 hours, and returns strictly valid JSON.
- **Google Dorking instead of direct scraping.** LinkedIn blocks direct unauthorized requests, so Manus searches via Google and Bing using `site:linkedin.com/jobs` plus filters. This is legal and reliable.
- **Push model over polling.** Having the agent call the webhook itself once done avoided wasting Make.com operations on repeated status checks.
- Dropped an unnecessary Parse JSON module in the Receiver scenario once it became clear the Router could read the webhook output directly, and fixed the Iterator mapping syntax (`{{64.value[1]}}`) during testing.

### Implementation Stages

1. Setup: Telegram bot plus a Manus AI project configured with the hard-filter system prompt.
2. Build the Launcher scenario.
3. Build the Receiver scenario, including the Router/Iterator fix above.
4. End-to-end testing and validation.

### Links

- Presentation: https://agentic-job-search.netlify.app/
- Live demo: not applicable. This is an internal automation triggered through Telegram rather than a browsable web app.
- GitHub: not published as a standalone public repo.

### Status

Complete.

---

# FILE: 02-agbu-final-projects/portfolio-website.md

## Portfolio Website

AGBU final project 2. Program: AI Automation / Agentic AI, AGBU Women Coders Program, ARDY Academy, Yerevan. Graduated with distinction, June 24, 2026.

### Goal

Build a professional portfolio site for Travel Tech + AI that functions as a live digital identity: it showcases 12 projects and lab experiments, includes a bio and skills section, and is managed through a real-time admin dashboard with email notifications, analytics, and full GitHub version control, deployed to a permanent production URL.

### Tech Stack and Why

- **Next.js 14 (App Router)**: frontend foundation, chosen for server-side rendering, file-based routing, and TypeScript support, which is the production-grade standard for a portfolio meant to represent real engineering ability.
- **Supabase**: PostgreSQL database, storage, and edge functions on the free tier (500MB database, 1GB storage, 50,000 requests/month), with native Make.com integration and row-level security.
- **Replit Deployments (Autoscale, 2 vCPU / 4GiB RAM)**: gives a permanent public URL, managed environment secrets, and zero-config Next.js deployment.
- **Resend + Supabase Edge Functions**: email notifications on a Deno serverless runtime. The contact form inserts a row into the messages table, which triggers an edge function that calls the Resend API to send a real-time email.
- **Umami Analytics**: open source, privacy-first, GDPR-compliant, and cookie-free. Added with a single script tag in layout.tsx, with the dashboard surfaced inside the Admin panel.
- **GitHub (Lilli-Ai/la-portfolio)**: version control and security baseline. All `.env*` files are wildcarded in .gitignore so no key ever reaches the repo.

### Architecture

Frontend: Next.js 14 App Router with TypeScript and inline styles. Database: Supabase PostgreSQL with four tables (projects, lab_items, messages, settings). Storage: a Supabase Storage bucket named `cv` for CV uploads without requiring a redeploy. Serverless: a Supabase Edge Function (`send-notification`) running on Deno. Analytics: Umami, integrated into the Admin dashboard. Deployment: Replit Autoscale, live at https://lilia-ai.replit.app.

### Key Engineering Decisions

- **Row-level security (RLS):** public read access, with writes allowed only through the service key.
- **CORS handling in the edge function:** `Access-Control-Allow-Origin: *` plus a preflight OPTIONS handler. Without this, the browser blocked requests coming from the Replit domain.
- **Environment secrets kept out of code:** the Resend API key lives in Supabase Secrets, and Supabase keys live in Replit Deployment Secrets.
- **Custom brand identity:** a custom favicon SVG using LA initials on a dark background (#0A0A0F) with a gold accent (#C9A227).
- **Open Graph SEO:** metadata configured in layout.tsx (og:title, og:description, og:url, Twitter Card) for clean link previews when shared on LinkedIn.

### Implementation Stages

1. Planning and architecture: tech stack, design system (dark theme with gold accent, Space Grotesk font, six pages).
2. Frontend build: navigation, footer, avatar, page background, and contact form components, plus CSS keyframe animations, deployed to Replit.
3. Supabase backend: four-table PostgreSQL schema, RLS policies, and the `cv` storage bucket.
4. Content: descriptions, tags, and links for 12 projects, bio, competency map, and a Lab section with transparent project statuses.
5. Admin dashboard: password-protected `/admin` route with tabs for Projects (CRUD), Messages, Lab, and CV.
6. Email notifications: contact form to edge function to Resend, with CORS handling and two email scenarios.
7. Analytics, SEO, and favicon.
8. GitHub and version control: private repository, with 10 public repos linked from the profile.
9. Deployment: Replit Autoscale, production URL, build and start on port 3000 via pnpm.

### Links

- Live demo: https://lilia-ai.replit.app
- GitHub: Lilli-Ai/la-portfolio
- Presentation: https://la-portfolio-slides.netlify.app/

### Status

Complete.

---

# FILE: 02-agbu-final-projects/traveltech-insights.md

## TravelTech Insights with AI Chatbot

AGBU final project 3. Program: AI Automation / Agentic AI, AGBU Women Coders Program, ARDY Academy, Yerevan. Graduated with distinction, June 24, 2026.

### Goal

Automated dashboard that independently collects, analyzes, and displays the latest AI and automation news from the Travel Tech industry, with no manual searching or updating required. An integrated AI chatbot (Typebot to n8n to Groq's Llama 3.3 70B) lets users ask Travel Tech questions and get real-time answers.

### Tech Stack and Why

- **n8n**: no-code/low-code automation platform, chosen to build complex pipelines without writing custom backend code, using ready-made service integrations.
- **SerpApi**: Google Search API used for article discovery, returning structured results (title, URL, date).
- **Firecrawl**: web scraping tool that extracts only the main article text, stripping out ads and navigation menus.
- **Postman**: used to test each service (SerpApi, Firecrawl, Airtable) independently before wiring them into n8n, following the practice of testing a service in isolation before integrating it.
- **Airtable**: chosen over a plain JSON file as a no-code database, to demonstrate structured storage with a native n8n integration. Stores Title, URL, Summary, and Date.
- **Groq with Llama 3.3 70B**: OpenRouter was evaluated first for vendor flexibility, but its free tier hit 429 rate limits. The architectural call was to switch to Groq for stable, unlimited free inference.
- **Typebot**: no-code chatbot builder with a simple visual constructor, embeddable via iframe anywhere.
- **Gradio on Hugging Face Spaces**: used for fast Python web interfaces with a simple, free deployment path.

### Architecture

Two-tab Hugging Face Space built with Gradio: an AI Assistant tab and an Insights Dashboard tab.

**Chatbot flow:** Typebot collects the user's question, sends it via webhook to n8n, which calls Groq's Llama 3.3 70B to generate a reply, then returns the answer back to Typebot.

**Data pipeline:** a manual trigger in n8n starts a SerpApi search for "AI automation travel tech 2026," results are split out individually, Firecrawl scrapes the full article text for each one, and the cleaned data is saved to Airtable. Each step was tested independently in Postman before being wired into the n8n flow.

**Dashboard:** `app.py` reads the data from Airtable via its API, a `clean_text()` function strips markdown noise, and the dashboard displays Title, URL, Summary, and Date for each article.

### Key Engineering Decisions

- Testing each API (SerpApi, Firecrawl, Airtable) in Postman before integration, to isolate failures early.
- Switching from OpenRouter to Groq after hitting free-tier rate limits, prioritizing reliability over the original vendor choice.
- Embedding Typebot via iframe directly inside the Hugging Face Space rather than hosting the chatbot separately, to keep the whole experience in one place.
- Keeping the Airtable token in Hugging Face Secrets rather than in code, and making the Space public only after that was in place.

### Implementation Stages

1. Infrastructure: Hugging Face Space with Gradio, split into AI Assistant and Insights Dashboard tabs.
2. AI chatbot: Typebot to webhook to n8n to Groq, with Llama 3.3 70B generating the reply and returning it to Typebot.
3. Data pipeline: manual trigger, SerpApi search, Split Out, Firecrawl scraping, Airtable storage, with each step tested in Postman.
4. Dashboard: `app.py` reads Airtable via API, cleans text, and displays results.
5. Final polish: Typebot embedded via iframe, Airtable token secured via Hugging Face Secrets, Space made public.

### Links

- Live demo: https://huggingface.co/spaces/liliaavagyan/TravelTech-AI-Insights
- Presentation: https://ai-insights-travel.netlify.app/
- GitHub: not published as a standalone public repo.

### Status

Complete.

---

# FILE: 03-client-work/tourism-booking-system.md

## Tourism Booking System

**Training exercise: mock client delivery simulation.** This project is a full dress rehearsal for a real client handover, carried out in a fully isolated environment: new email, new GitHub organization, new Neon and Replit instances. No real client, real business, or real credentials were involved at any point.

### Goal

Deliver a fully functional booking system with configured infrastructure, practicing autonomous management and scalability for future growth, as a complete and professional handover package.

### Tech Stack and Why

Built on a code-first approach with no vendor lock-in:

- **Replit (Next.js)**: hosting environment, chosen for full control over the server and configuration.
- **GitHub**: version control, used as the centralized repository for the training organization.
- **Neon PostgreSQL**: cloud database, chosen for reliable storage with ACID transactions.

| Component | Technology | Purpose |
|---|---|---|
| Backend API | Next.js Route Handlers | Request processing under `/portal/` |
| Frontend UI | React (Next.js) | Business administration interface |
| Database | PostgreSQL (Neon) | Data management for bookings, trips, and clients |
| Data Flow | CRUD operations | Sync between database and UI |

### Architecture

The project follows three principles: technological independence (fully autonomous, deployable on any cloud hosting provider), transparency (the entire codebase is open for audit and direct modification, with no dependency on third-party AI builders), and scalability (new modules can be added as the business grows).

Data model centers on three entities: Bookings, Trips, and Clients, each carrying metadata. Booking activity automatically triggers customer profile updates. Admin tools cover status management, tour modules, and analytics.

### Key Engineering Decisions

- SSL-required database connections (`sslmode=require`) for all traffic to Neon.
- Credentials handled through a secure delivery structure as part of handover practice, not stored in the codebase.
- Full administrative access transfer practiced end to end, including a handover checklist: rotate credentials, enable 2FA, verify access rights, and archive the delivery package.
- Redis caching and SQL views identified as the recommended next steps for scaling.
- GitHub duplication plus periodic SQL dumps recommended for disaster recovery.

### Visual Evidence (from Project Visuals)

- Neon database table view (`tourism-db`, public schema with bookings, clients, and trips tables).
- Admin access login screen ("Travel Portal: Staff Only").
- Analytics Overview dashboard: Total Bookings, Total Clients, Total Trips, Bookings by Status, Status Counts.
- GitHub repository view showing commit history and the repo description: "Tourism agency booking management dashboard with automated AI analysis and audit logging" (tagged react, nextjs, postgresql, data-management, system-architecture, code-first, booking-system, travel-management, saas-application, replit, fullstack-app, neon-db, tourism-tech).

### Links

- Live demo (training instance): https://terra-flow.replit.app
- GitHub (training organization): https://github.com/Tourism-Project-2026/tourism-booking-system

This repository lives under its own organization (Tourism-Project-2026) rather than my personal GitHub account, a deliberate choice that keeps it isolated from personal projects and makes ownership easy to fork or transfer to a client, mirroring how a real handover would work.

### Status

Complete, as a training exercise. No production deployment or real client data.

---

# FILE: 04-skills-matrix.md

## Skills Matrix

Summary of tools and skills demonstrated across the 19 course projects, 3 AGBU final projects, and the tourism booking system training exercise.

### No-Code and Low-Code App Building

| Tool | Used In |
|---|---|
| Opal (Google) | Beth Hart Live Experience, Explorer Syunik, Homework AI Tracker |
| Lovable | Syunik Cinematic Travel Guide, Curated Hiking Trails in Armenia |
| Bolt.new | Vayots Dzor: the Ancient Wine Cradle |
| Vercel / v0 | Yerevan Secrets |
| Create.xyz | Armenian Music Box |
| Replit | Armenian Stone Alphabet, Budget Planner, Portfolio-Backend, Portfolio Website, Tourism Booking System |
| Gamma | Website for a New Tour Agency |
| Manus AI | AI Portfolio Projects, Job Board Automation (agentic search) |
| Render | AI Resume Analyzer |
| Cloudflare Workers | Lost & Found Hub |

### Automation and Orchestration

| Tool | Used In |
|---|---|
| Make.com | Telegram AI Assistant, Job Board Automation |
| n8n | TravelTech Insights |
| Google Apps Script | Homework AI Tracker, YouTube Researcher Agent |

### AI and LLM Integration

| Tool / Model | Used In |
|---|---|
| OpenAI / Anthropic APIs | Telegram AI Assistant |
| Google Gemini API | AI Resume Analyzer |
| Groq + Llama 3.3 70B | TravelTech Insights chatbot |
| Manus AI (agentic web search) | Job Board Automation |
| Comet (agentic browser) | Agentic Browser Scenario (Visa Helper) |

### Full-Stack Development

| Technology | Used In |
|---|---|
| Next.js / React | Portfolio Website, Yerevan Secrets, Tourism Booking System |
| TypeScript | Curated Hiking Trails, Armenian Stone Alphabet, Budget Planner, Portfolio-Backend |
| Python / FastAPI | AI Resume Analyzer, TravelTech Insights dashboard |
| Node.js | AI Portfolio Projects |

### Databases and Storage

| Technology | Used In |
|---|---|
| PostgreSQL (Supabase) | Portfolio Website |
| PostgreSQL (Neon) | Tourism Booking System |
| Airtable | TravelTech Insights |
| Google Sheets | Homework AI Tracker, YouTube Researcher Agent, Job Board Automation, Telegram AI Assistant |
| MySQL | AI Portfolio Projects |

### Chatbots and Conversational Interfaces

| Tool | Used In |
|---|---|
| Telegram Bot API | Telegram AI Assistant, Job Board Automation |
| Typebot | TravelTech Insights |
| Botpress | Lost & Found Hub |

### Analytics, Security, and Handover Practices

| Skill | Demonstrated In |
|---|---|
| Umami Analytics integration | Portfolio Website |
| Row-level security (RLS) | Portfolio Website |
| Environment secrets management | Portfolio Website, TravelTech Insights, Tourism Booking System |
| SSL-enforced database connections | Tourism Booking System |
| Credential rotation and access-handover checklists | Tourism Booking System |
| API testing discipline (Postman before integration) | TravelTech Insights |
| SEO and Open Graph metadata | Portfolio Website |

### Web APIs and Search

| Tool | Used In |
|---|---|
| SerpApi | TravelTech Insights |
| Firecrawl | TravelTech Insights |
| RapidAPI (YouTube Search) | YouTube Researcher Agent |
| Google Dorking / X-Ray search | Job Board Automation |

---

# FILE: 05-timeline.md

## Timeline

**April 15, 2026: Course start.** Began the AI Automation / Agentic AI track of the AGBU Women Coders Program at ARDY Academy in Yerevan. Goal: build AI-powered applications using no-code and low-code tools.

**April 15 – June 17, 2026: Coursework.** Completed 32 hours of instruction and 19 hands-on mini-projects across Opal, Lovable, Bolt.new, Vercel, Create.xyz, Replit, Make.com, Google Apps Script, Hugging Face, Cloudflare, and other platforms.

**June 24, 2026: Graduation.** Presented three final projects (Job Board Automation, Portfolio Website, and TravelTech Insights) to roughly 20 students and the AGBU organizers. Graduated with distinction.

**Post-graduation: Advanced course and training exercise.** Enrolled in an advanced follow-up course. Set up a fully isolated environment (new email, new GitHub organization, new Neon and Replit instances) to run a complete mock client delivery, the Tourism Booking System, as hands-on practice for real client handovers.

**July 2026: Present.** Building this personal knowledge base to consolidate the full journey, while transitioning into Travel Tech, combining a background in tourism and customer experience with AI automation skills.
