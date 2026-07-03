# TravelTech Insights with AI Chatbot

AGBU final project 3. Program: AI Automation / Agentic AI, AGBU Women Coders Program, ARDY Academy, Yerevan. Graduated with distinction, June 24, 2026.

## Goal

Automated dashboard that independently collects, analyzes, and displays the latest AI and automation news from the Travel Tech industry, with no manual searching or updating required. An integrated AI chatbot (Typebot to n8n to Groq's Llama 3.3 70B) lets users ask Travel Tech questions and get real-time answers.

## Tech Stack and Why

- **n8n**: no-code/low-code automation platform, chosen to build complex pipelines without writing custom backend code, using ready-made service integrations.
- **SerpApi**: Google Search API used for article discovery, returning structured results (title, URL, date).
- **Firecrawl**: web scraping tool that extracts only the main article text, stripping out ads and navigation menus.
- **Postman**: used to test each service (SerpApi, Firecrawl, Airtable) independently before wiring them into n8n, following the practice of testing a service in isolation before integrating it.
- **Airtable**: chosen over a plain JSON file as a no-code database, to demonstrate structured storage with a native n8n integration. Stores Title, URL, Summary, and Date.
- **Groq with Llama 3.3 70B**: OpenRouter was evaluated first for vendor flexibility, but its free tier hit 429 rate limits. The architectural call was to switch to Groq for stable, unlimited free inference.
- **Typebot**: no-code chatbot builder with a simple visual constructor, embeddable via iframe anywhere.
- **Gradio on Hugging Face Spaces**: used for fast Python web interfaces with a simple, free deployment path.

## Architecture

Two-tab Hugging Face Space built with Gradio: an AI Assistant tab and an Insights Dashboard tab.

**Chatbot flow:** Typebot collects the user's question, sends it via webhook to n8n, which calls Groq's Llama 3.3 70B to generate a reply, then returns the answer back to Typebot.

**Data pipeline:** a manual trigger in n8n starts a SerpApi search for "AI automation travel tech 2026," results are split out individually, Firecrawl scrapes the full article text for each one, and the cleaned data is saved to Airtable. Each step was tested independently in Postman before being wired into the n8n flow.

**Dashboard:** `app.py` reads the data from Airtable via its API, a `clean_text()` function strips markdown noise, and the dashboard displays Title, URL, Summary, and Date for each article.

## Key Engineering Decisions

- Testing each API (SerpApi, Firecrawl, Airtable) in Postman before integration, to isolate failures early.
- Switching from OpenRouter to Groq after hitting free-tier rate limits, prioritizing reliability over the original vendor choice.
- Embedding Typebot via iframe directly inside the Hugging Face Space rather than hosting the chatbot separately, to keep the whole experience in one place.
- Keeping the Airtable token in Hugging Face Secrets rather than in code, and making the Space public only after that was in place.

## Implementation Stages

1. Infrastructure: Hugging Face Space with Gradio, split into AI Assistant and Insights Dashboard tabs.
2. AI chatbot: Typebot to webhook to n8n to Groq, with Llama 3.3 70B generating the reply and returning it to Typebot.
3. Data pipeline: manual trigger, SerpApi search, Split Out, Firecrawl scraping, Airtable storage, with each step tested in Postman.
4. Dashboard: `app.py` reads Airtable via API, cleans text, and displays results.
5. Final polish: Typebot embedded via iframe, Airtable token secured via Hugging Face Secrets, Space made public.

## Links

- Live demo: https://huggingface.co/spaces/liliaavagyan/TravelTech-AI-Insights
- Presentation: https://ai-insights-travel.netlify.app/
- GitHub: not published as a standalone public repo.

## Status

Complete.
