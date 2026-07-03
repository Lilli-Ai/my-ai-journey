# AI-Powered Job Board Automation

AGBU final project 1. Program: AI Automation / Agentic AI, AGBU Women Coders Program, ARDY Academy, Yerevan. Graduated with distinction, June 24, 2026.

## Goal

Automated pipeline that finds Junior and Entry-level AI Automation and Agentic AI job postings, triggered by a single Telegram button, and returns only results posted in the last 24 hours.

## Tech Stack and Why

- **Manus AI**: autonomous web agent. Used to perform Google Dorking (X-Ray search), which makes LinkedIn's closed job pages reachable through Google's public index. This is a legal search method, not scraping, and Manus provides a visual reasoning log showing its full thought process.
- **Make.com**: orchestration layer, split into two scenarios to support an async architecture: Manus_Job_Launcher and Manus_Data_Receiver.
- **Google Sheets**: results hub, chosen for its native Make.com integration. Two sheets are used: Global Remote (LinkedIn worldwide) and Armenia Local (LinkedIn Armenia, Staff.am, and Job.am).
- **Telegram Bot**: the trigger is a single /search command button rather than free text input, which keeps the interaction simple and saves Make.com operation credits.

## Architecture

The pipeline is split into two independent Make.com scenarios rather than one, because a single scenario hit Make.com's 40-60 second timeout window while the agent was still thinking.

- **Scenario 1: Manus_Job_Launcher:** Telegram (Watch Updates) → filter for the /search command → HTTP POST to the Manus API's task.create endpoint, including a webhook_url for the callback.
- **Scenario 2: Manus_Data_Receiver:** waits on the webhook. Once Manus finishes its search, it posts the results to that webhook. A Router splits the flow into global_remote and armenia_local branches. An Iterator opens the results array, and Google Sheets "Add a Row" writes each vacancy.

This is a push model: the Launcher fires the request and releases immediately rather than waiting for a reply. Manus contacts the Receiver on its own when the results are ready. Full flow: Telegram → Launcher → Manus AI → Receiver → Google Sheets.

## Key Engineering Decisions

- **Hard filters live in the Manus system prompt**, not downstream in Make.com. Manus owns all data-cleanliness responsibility: it rejects Senior/Mid-level roles, postings requiring an EU/US work permit, and anything older than 24 hours, and returns strictly valid JSON.
- **Google Dorking instead of direct scraping.** LinkedIn blocks direct unauthorized requests, so Manus searches via Google and Bing using `site:linkedin.com/jobs` plus filters. This is legal and reliable.
- **Push model over polling.** Having the agent call the webhook itself once done avoided wasting Make.com operations on repeated status checks.
- Dropped an unnecessary Parse JSON module in the Receiver scenario once it became clear the Router could read the webhook output directly, and fixed the Iterator mapping syntax (`{{64.value[1]}}`) during testing.

## Implementation Stages

1. Setup: Telegram bot plus a Manus AI project configured with the hard-filter system prompt.
2. Build the Launcher scenario.
3. Build the Receiver scenario, including the Router/Iterator fix above.
4. End-to-end testing and validation.

## Links

- Presentation: https://agentic-job-search.netlify.app/
- Live demo: not applicable. This is an internal automation triggered through Telegram rather than a browsable web app.
- GitHub: not published as a standalone public repo.

## Status

Complete.
