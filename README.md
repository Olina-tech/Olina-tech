<div align="center">

# Olina

### Backend infrastructure for AI-built apps

**Olina gives developers, AI agents, and software platforms a single control plane to create and manage production-ready backends.**

Database · Authentication · Storage · Realtime · APIs · Environments

[Website](https://olina.tech) · [GitHub](https://github.com/Olina-tech)

[![X](https://img.shields.io/badge/X-@olinatech-111111?style=flat-square&logo=x)](https://x.com/olinatech)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Olina_Tech-0A66C2?style=flat-square&logo=linkedin)](https://www.linkedin.com/company/olina-tech)
[![GitHub](https://img.shields.io/badge/GitHub-Olina--tech-181717?style=flat-square&logo=github)](https://github.com/Olina-tech)

</div>

---

## What is Olina?

Modern AI coding tools can generate applications quickly, but every generated app still needs reliable backend infrastructure: data, identity, files, APIs, realtime events, isolation, usage controls, and lifecycle management.

Olina is building the backend control plane for that workflow.

Instead of wiring multiple infrastructure services together, a developer or AI agent should be able to request an environment and receive a ready-to-use backend through one API.

```text
Developer / AI Agent
        │
        ▼
      Olina
        │
        ├── Database
        ├── Authentication
        ├── Storage
        ├── Realtime
        ├── APIs
        └── Isolated environments
```

> Build the app. Olina handles the backend.

## Who Olina is for

Olina is designed for:

- AI coding platforms and app builders
- AI agents that need temporary or isolated backend environments
- SaaS teams that want repeatable development and preview environments
- developers who want one programmable backend lifecycle
- platforms that need backend infrastructure provisioned for each customer, workspace, or generated application

## Core product

### Instant backend environments

Create a backend environment programmatically and receive the credentials and endpoints needed by an application or agent.

```bash
olina create my-app
```

Conceptually, an Olina environment can provide:

```text
✓ Relational database
✓ Authentication
✓ File storage
✓ Realtime services
✓ Application APIs
✓ Environment credentials
```

### Environment lifecycle

Olina is designed around programmable lifecycle operations instead of manual infrastructure setup.

```text
Create → Configure → Use → Clone → Reset → Destroy
```

This is especially useful for AI agents, tests, previews, generated applications, and short-lived development work.

### Agent-ready infrastructure

AI agents should be able to safely request infrastructure without receiving unrestricted control over an organization's production systems.

Olina's direction includes:

- isolated environments per task or agent
- scoped credentials
- expiration and automatic cleanup
- quotas and usage controls
- auditability
- safe development and migration workflows

## Platform architecture

The public Olina architecture is intentionally provider-agnostic. Applications integrate with Olina rather than directly depending on the infrastructure providers behind it.

```text
Users / Developers / AI Agents
             │
             ▼
        Olina Edge
             │
             ▼
        Olina API
             │
      ┌──────┴──────┐
      │ Control Plane│
      └──────┬──────┘
             │
   ┌─────────┼─────────┐
   ▼         ▼         ▼
Database   Identity   Storage
   │         │         │
   └──── Realtime / APIs ────┐
                             │
                       Usage & Billing
```

The goal is a stable Olina API and developer experience while keeping the infrastructure implementation replaceable and evolvable behind the control plane.

## API direction

Olina is API-first. The control surface is designed for both humans and autonomous software.

```http
POST   /v1/projects
GET    /v1/projects/:id
POST   /v1/projects/:id/environments
GET    /v1/environments/:id
POST   /v1/environments/:id/clone
POST   /v1/environments/:id/reset
DELETE /v1/environments/:id
```

The exact API is under active development and may change before general availability.

## Domain structure

Olina's product domains are organized around a clear separation between the company site, control plane, documentation, and customer-facing endpoints.

```text
olina.tech                 Company website
console.olina.tech         User control panel
api.olina.tech             Olina control-plane API
docs.olina.tech            Developer documentation
status.olina.tech          Service status

<project>.api.olina.tech   Project API endpoint
<project>.app.olina.tech   Application endpoint
<project>.files.olina.tech File endpoint
```

Not every endpoint listed above is necessarily publicly available yet.

## Business model

Olina is being built as a paid infrastructure platform. The business model combines platform subscriptions with usage-based billing for backend resources and higher-volume platform workloads.

The product is intentionally not designed around an unlimited permanent free infrastructure tier.

Expected customer segments include individual developers, growing software teams, AI app builders, and platforms that provision large numbers of environments programmatically.

## What makes Olina different

Olina is not intended to be another dashboard wrapped around a database.

The product is focused on the orchestration layer between AI-generated software and production backend infrastructure:

- one API for the backend lifecycle
- infrastructure that AI agents can safely create and destroy
- disposable and isolated environments
- provider abstraction behind Olina-owned interfaces
- usage controls and billing at the Olina layer
- developer tooling designed for programmatic workflows

This control plane is the product.

## Development principles

### Provider abstraction

Customer applications integrate with Olina interfaces instead of being coupled to a single underlying infrastructure provider.

### Secure by default

Credentials should be scoped, secrets should not be exposed unnecessarily, and destructive operations should be auditable.

### API first

Anything important in the console should ultimately be automatable through the Olina API.

### Simple developer experience

Infrastructure complexity belongs behind the platform, not in the customer's application.

### Usage-aware

Infrastructure has real cost. Resource creation, quotas, metering, and cleanup are first-class parts of the product.

## Roadmap

| Phase | Objective |
|---|---|
| **Foundation** | Identity, organizations, projects, API keys, billing model and control-plane data model |
| **MVP** | Create and delete isolated backend environments through the Olina API |
| **Developer experience** | Console, CLI, logs, credentials, usage views and documentation |
| **Agent workflows** | TTL environments, automatic cleanup, scoped agent access and lifecycle automation |
| **Platform integrations** | SDKs, webhooks, CI/CD and AI-builder integrations |
| **Scale** | Advanced isolation, policy controls, observability and enterprise capabilities |

## Current status

Olina is in active development. Public repositories, APIs, product names, limits, and architecture may evolve as the platform is validated with real developer and AI-agent workflows.

## Security

Please do not disclose suspected vulnerabilities through a public GitHub issue.

Send security reports with reproduction steps, impact, and sanitized evidence to **security@olina.tech**.

## Company

Olina is a product of **Sirmint Technologies**.

For partnerships, platform integrations, and business inquiries: **hello@olina.tech**

## Connect

- [olina.tech](https://olina.tech)
- [X — @olinatech](https://x.com/olinatech)
- [LinkedIn — Olina Tech](https://www.linkedin.com/company/olina-tech)
- [GitHub — Olina-tech](https://github.com/Olina-tech)

---

<div align="center">

### Backend infrastructure for the software AI builds.

© 2026 Sirmint Technologies · Olina

</div>
