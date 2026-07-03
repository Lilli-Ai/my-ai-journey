# Tourism Booking System

**Training exercise: mock client delivery simulation.** This project is a full dress rehearsal for a real client handover, carried out in a fully isolated environment: new email, new GitHub organization, new Neon and Replit instances. No real client, real business, or real credentials were involved at any point.

## Goal

Deliver a fully functional booking system with configured infrastructure, practicing autonomous management and scalability for future growth, as a complete and professional handover package.

## Tech Stack and Why

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

## Architecture

The project follows three principles: technological independence (fully autonomous, deployable on any cloud hosting provider), transparency (the entire codebase is open for audit and direct modification, with no dependency on third-party AI builders), and scalability (new modules can be added as the business grows).

Data model centers on three entities: Bookings, Trips, and Clients, each carrying metadata. Booking activity automatically triggers customer profile updates. Admin tools cover status management, tour modules, and analytics.

## Key Engineering Decisions

- SSL-required database connections (`sslmode=require`) for all traffic to Neon.
- Credentials handled through a secure delivery structure as part of handover practice, not stored in the codebase.
- Full administrative access transfer practiced end to end, including a handover checklist: rotate credentials, enable 2FA, verify access rights, and archive the delivery package.
- Redis caching and SQL views identified as the recommended next steps for scaling.
- GitHub duplication plus periodic SQL dumps recommended for disaster recovery.

## Visual Evidence (from Project Visuals)

- Neon database table view (`tourism-db`, public schema with bookings, clients, and trips tables).
- Admin access login screen ("Travel Portal: Staff Only").
- Analytics Overview dashboard: Total Bookings, Total Clients, Total Trips, Bookings by Status, Status Counts.
- GitHub repository view showing commit history and the repo description: "Tourism agency booking management dashboard with automated AI analysis and audit logging" (tagged react, nextjs, postgresql, data-management, system-architecture, code-first, booking-system, travel-management, saas-application, replit, fullstack-app, neon-db, tourism-tech).

## Links

- Live demo (training instance): https://terra-flow.replit.app
- GitHub (training organization): https://github.com/Tourism-Project-2026/tourism-booking-system

This repository lives under its own organization (Tourism-Project-2026) rather than my personal GitHub account, a deliberate choice that keeps it isolated from personal projects and makes ownership easy to fork or transfer to a client, mirroring how a real handover would work.

## Status

Complete, as a training exercise. No production deployment or real client data.
