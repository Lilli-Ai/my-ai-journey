# Portfolio Website

AGBU final project 2. Program: AI Automation / Agentic AI, AGBU Women Coders Program, ARDY Academy, Yerevan. Graduated with distinction, June 24, 2026.

## Goal

Build a professional portfolio site for Travel Tech + AI that functions as a live digital identity: it showcases 12 projects and lab experiments, includes a bio and skills section, and is managed through a real-time admin dashboard with email notifications, analytics, and full GitHub version control, deployed to a permanent production URL.

## Tech Stack and Why

- **Next.js 14 (App Router)**: frontend foundation, chosen for server-side rendering, file-based routing, and TypeScript support, which is the production-grade standard for a portfolio meant to represent real engineering ability.
- **Supabase**: PostgreSQL database, storage, and edge functions on the free tier (500MB database, 1GB storage, 50,000 requests/month), with native Make.com integration and row-level security.
- **Replit Deployments (Autoscale, 2 vCPU / 4GiB RAM)**: gives a permanent public URL, managed environment secrets, and zero-config Next.js deployment.
- **Resend + Supabase Edge Functions**: email notifications on a Deno serverless runtime. The contact form inserts a row into the messages table, which triggers an edge function that calls the Resend API to send a real-time email.
- **Umami Analytics**: open source, privacy-first, GDPR-compliant, and cookie-free. Added with a single script tag in layout.tsx, with the dashboard surfaced inside the Admin panel.
- **GitHub (Lilli-Ai/la-portfolio)**: version control and security baseline. All `.env*` files are wildcarded in .gitignore so no key ever reaches the repo.

## Architecture

Frontend: Next.js 14 App Router with TypeScript and inline styles. Database: Supabase PostgreSQL with four tables (projects, lab_items, messages, settings). Storage: a Supabase Storage bucket named `cv` for CV uploads without requiring a redeploy. Serverless: a Supabase Edge Function (`send-notification`) running on Deno. Analytics: Umami, integrated into the Admin dashboard. Deployment: Replit Autoscale, live at https://lilia-ai.replit.app.

## Key Engineering Decisions

- **Row-level security (RLS):** public read access, with writes allowed only through the service key.
- **CORS handling in the edge function:** `Access-Control-Allow-Origin: *` plus a preflight OPTIONS handler. Without this, the browser blocked requests coming from the Replit domain.
- **Environment secrets kept out of code:** the Resend API key lives in Supabase Secrets, and Supabase keys live in Replit Deployment Secrets.
- **Custom brand identity:** a custom favicon SVG using LA initials on a dark background (#0A0A0F) with a gold accent (#C9A227).
- **Open Graph SEO:** metadata configured in layout.tsx (og:title, og:description, og:url, Twitter Card) for clean link previews when shared on LinkedIn.

## Implementation Stages

1. Planning and architecture: tech stack, design system (dark theme with gold accent, Space Grotesk font, six pages).
2. Frontend build: navigation, footer, avatar, page background, and contact form components, plus CSS keyframe animations, deployed to Replit.
3. Supabase backend: four-table PostgreSQL schema, RLS policies, and the `cv` storage bucket.
4. Content: descriptions, tags, and links for 12 projects, bio, competency map, and a Lab section with transparent project statuses.
5. Admin dashboard: password-protected `/admin` route with tabs for Projects (CRUD), Messages, Lab, and CV.
6. Email notifications: contact form to edge function to Resend, with CORS handling and two email scenarios.
7. Analytics, SEO, and favicon.
8. GitHub and version control: private repository, with 10 public repos linked from the profile.
9. Deployment: Replit Autoscale, production URL, build and start on port 3000 via pnpm.

## Links

- Live demo: https://lilia-ai.replit.app
- GitHub: Lilli-Ai/la-portfolio
- Presentation: https://la-portfolio-slides.netlify.app/

## Status

Complete.
