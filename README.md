## Alpay Sahin

Fullstack Developer focused on TypeScript Backends, Multi Tenant SaaS and Access Control architectures. Since August 2025 main maintainer of two SaaS products in production. Backend, Frontend and customer communication are part of my scope.

---

### Stack

| Area | Technologies |
|---|---|
| Backend | TypeScript, NestJS, Prisma, PostgreSQL, Redis, GraphQL, REST |
| Frontend | React, Vite, styled-components, TanStack Query, Apollo |
| Infra | AWS S3, Docker, Hetzner, GitHub Actions, GitLab CI |

---

### Focus

Multi Tenant architectures, Row Level Security as Prisma Middleware, Request scoped Context via AsyncLocalStorage, grant based Permission Models and pragmatic Auth flows without overengineering.

---

### Current work context

#### CAFM SaaS Platform

In production use by multiple corporations and companies. Shortly after I joined I received the handover from the CTO and have been the main maintainer since. My scope covers architecture and implementation, onboarding new colleagues and direct customer contact via meetings and the Featurebase ticket system.

Larger features and subsystems:

- Row Level Security as Prisma Middleware. Intercepts every database access and resolves chained table relations. Entities and Controllers are scanned at field level and the matching filter conditions are injected automatically into the queries.
- Permission System with around 100 grants, combined with Guards and an AsyncLocalStorage Request Context. The authenticated User is isolated per request and carried through the entire flow.
- PostgreSQL Session Variables for Audit Trails directly at the database level.
- Ticket system with Kanban backend and Cronjobs.
- File transfer via AWS S3 with Presigned URLs. On the frontend a props driven component reused in multiple places.
- Migration of the legacy Node backend to NestJS. Datasets in the six digit range were brought to acceptable response times via pagination and query tuning.

48 of the 100 plus backend modules in the codebase show active changes from me.

#### Watch Capital Platform (parallel product)

NestJS backend with two React frontends for customers and admins. I refactored the platform end to end and extended it with new features. Backend, both frontends and customer communication are on me.

Larger features and subsystems:

- Drag and Drop system for watch management in iOS style. Long press switches the tiles into wiggle mode for free arrangement. Dragging two entries onto each other creates a group. Existing groups accept additional watches via drop, and individual entries can be dragged out of a group again.
- Verification system with five stage status workflow, live chat between customer and admin and email notifications on transitions.
- Internationalization of both frontends via i18next with a global `i18n()` binding. Date and time are localized via Moment. Language switch at runtime without reload.
- Autocomplete based on a JSONB Distinct via a dynamic QueryBuilder.
- S3 image pipeline with eight image types per watch. Old versions are cleaned up automatically on upload.
- Modal based flows for creating new watches. Service and inventory watches use separate paths with their own validation.

---

### Featured Repositories

#### snio

Multi Tenant Esport Platform showcase project. NestJS, Prisma, React, Tailwind, Turborepo. Currently in active development with a transparent sprint roadmap. The repository demonstrates Row Level Security as Prisma Middleware, AsyncLocalStorage Request Context, grant based Permission System, JWT plus Refresh Rotation and a two server Hetzner Private Network deployment.

#### cv-tool (public soon)

React and Vite application for application documents with live preview and PDF export via the Chrome Print Pipeline. Multiple profiles are stored in localStorage. Legacy data is migrated automatically. The cover letter is composed modularly from three profile variants and swappable building blocks for intro and outro. styled-components, no backend, runs fully offline.

---

<details>
<summary><b>Other work</b></summary>

#### Discord Bot (private)

TypeScript with Prisma and Supabase. Bidirectional sync between Discord and database, including restore after Soft Delete. The Google Drive API integration runs via Service Account Auth and covers folder management, permission transfer and a TTL cache. Docker deployment on Hetzner and CI via GitHub Actions.

#### PDF Generator (private)

Rendering pipeline with Puppeteer and pdf-lib. A Screenshot Engine renders HTML at triple resolution into the PDF. For clickable tables of contents the tool generates native PDF link annotations and converts DOM coordinates to PDF coordinates.

</details>

---

### Contact

LinkedIn coming soon.
