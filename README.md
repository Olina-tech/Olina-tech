<div align="center">

# Olina

### Research intelligence infrastructure for scientific and R&D labs

**Olina is a product and deep-technology initiative of Sirmint Technologies.** We are building an evidence-first AI platform that helps research teams move from a scientific question to traceable, reproducible and decision-ready work.

[Website](https://olina.tech) · [Research App](https://aap.olina.tech) · [Workspace](https://workspace.olina.tech) · [Control Center](https://control.olina.tech)

[![X](https://img.shields.io/badge/X-@olinatech-111111?style=flat-square&logo=x)](https://x.com/olinatech)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Olina_Tech-0A66C2?style=flat-square&logo=linkedin)](https://www.linkedin.com/company/olina-tech)
[![Reddit](https://img.shields.io/badge/Reddit-olinatech-FF4500?style=flat-square&logo=reddit&logoColor=white)](https://www.reddit.com/user/olinatech/)
[![GitHub](https://img.shields.io/badge/GitHub-Olina--tech-181717?style=flat-square&logo=github)](https://github.com/Olina-tech)

</div>

---

## The problem

Scientific and R&D teams work across papers, experimental notes, datasets, conversations and disconnected software. General-purpose AI can produce fluent answers, but high-stakes research requires more:

- evidence that can be inspected
- citations that can be verified
- uncertainty that remains visible
- repeatable research workflows
- secure collaboration around private lab knowledge
- control over models, compute, access and cost

Olina is being built for that gap.

## Company

**Sirmint Technologies** is the parent company behind Olina. Sirmint Technologies develops and operates the Olina platform, products, infrastructure and research-model program.

Olina is the company's research-intelligence product family for scientific and R&D labs.

## Our vision

Our long-term vision is to become the research intelligence layer for labs: a shared system in which scientists and AI can investigate literature, compare competing findings, organize institutional knowledge and produce defensible research outputs.

We are not building another generic chatbot. We are building infrastructure for evidence-intensive work.

> From scientific question to defensible evidence.

## What Olina is building

### Olina Research

A deep-research application for literature investigation, source synthesis, citation-aware answers and structured reports.

### Olina Workspace

A collaborative knowledge environment for lab pages, research notes, projects, files and real-time team communication.

### Olina Control

An administration layer for organizations to manage members, permissions, compute, usage, billing, security and research operations.

### Olina API

A shared backend connecting identity, research jobs, files, AI inference, usage controls, payments and product integrations.

## Product portfolio

| Product | Repository | Role |
|---|---|---|
| **Olina Web** | [olina-web](https://github.com/Olina-tech/olina-web) | Company website, pricing, trust and legal information |
| **Olina Research** | [olina-app](https://github.com/Olina-tech/olina-app) | Evidence-first AI research experience |
| **Olina Workspace** | [olina-workspace](https://github.com/Olina-tech/olina-workspace) | Collaborative lab knowledge and project workspace |
| **Olina Control** | [olina-control](https://github.com/Olina-tech/olina-control) | Organization, compute, security and billing controls |
| **Olina API** | [olina-api](https://github.com/Olina-tech/olina-api) | Platform backend and AI orchestration layer |
| **Realtime Chat** | [realtime-chat-frontend](https://github.com/Olina-tech/realtime-chat-frontend) | Real-time research and team communication interface |

## The Olina research model strategy

Olina's defensibility will come from a research-specific intelligence system—not only from access to a general-purpose model.

### Stage 1 — Evidence infrastructure

- retrieval across papers and authorized lab documents
- source-preserving research pipelines
- citation and claim traceability
- structured reports and reusable research memory
- model routing with compute and cost controls

### Stage 2 — Proprietary specialist models

- paper relevance and reranking
- scientific claim extraction
- citation consistency checking
- conflicting-evidence detection
- methodology and research-risk classification
- experiment and protocol parsing

### Stage 3 — Olina Science Model

After building licensed, permissioned datasets and rigorous evaluations, we plan to fine-tune research-focused open models using parameter-efficient training. Continued pretraining or a larger proprietary model will be considered only when product usage, data quality and economics justify it.

The moat is the complete system: permissioned data, research workflows, specialist models, evaluations, retrieval, verification, governance and user feedback.

## Platform architecture

```text
Olina Web · Research · Workspace · Control
                       │
                   Olina API
                       │
       Research orchestration · AI gateway
                       │
  Supabase · D1 · R2 · Workers AI · Realtime
                       │
  Identity · Evidence · Files · Usage · Billing
```

### Infrastructure direction

- **Application:** React and modern responsive web interfaces
- **Edge/API:** Cloudflare Workers
- **AI:** Workers AI initially, with portable external GPU inference as required
- **Identity and relational data:** Supabase and PostgreSQL
- **Operational metadata:** Cloudflare D1
- **Research files and generated reports:** Cloudflare R2
- **Realtime collaboration:** RealtimeKit and product-level event services
- **Payments:** Creem with premium USD plans
- **Deployment principle:** provider-flexible compute across major cloud platforms when workload economics require it

## Trust by design

Labs should remain in control of their knowledge.

- private customer data is not used for model training by default
- training requires explicit permission and appropriate data rights
- source context and model uncertainty should remain visible
- access, usage and compute limits are organization-controlled
- sensitive files are isolated through authenticated storage boundaries
- research outputs require human verification before consequential use

Olina is research infrastructure, not a substitute for scientific judgment.

## Business model

Olina is designed as a premium B2B software and compute platform for labs and research-driven organizations.

Revenue is expected to combine:

- organization subscriptions in USD
- metered research and AI compute
- storage and collaboration capacity
- custom deployments and integrations
- dedicated enterprise security and support

The product is intentionally not positioned as an unlimited free AI service; deep research carries real inference, retrieval and storage costs.

## Execution roadmap

| Phase | Objective |
|---|---|
| **MVP** | Connect products through one API, identity layer and production data model |
| **Research foundation** | Deliver authenticated projects, files, research jobs, citations and reports |
| **Lab workspace** | Add collaborative documents, team rooms and institutional research memory |
| **Intelligence layer** | Introduce evaluation pipelines and proprietary specialist models |
| **Scale** | Add enterprise governance, dedicated capacity and global lab deployments |

Current repositories represent an actively developing platform. Features and interfaces will evolve as product validation continues.

## What we measure

Our product and model development will be evaluated against research outcomes—not chatbot fluency alone:

- citation correctness
- claim-to-source traceability
- evidence coverage
- contradiction detection
- researcher time saved
- report reproducibility
- inference cost per completed research task
- team adoption and retained research workflows

## Collaboration and investment

Olina's company, product development and investment relationships are led under **Sirmint Technologies**.

We want to work with research labs, scientific teams, design partners, infrastructure partners and investors who believe AI for science must be verifiable, controllable and built around real research workflows.

For partnerships, pilots and investment conversations: **hello@olina.tech**

## Security

Please do not disclose suspected vulnerabilities through a public GitHub issue. Send the affected service, reproduction steps, impact and sanitized evidence to **security@olina.tech**.

## Connect

- [olina.tech](https://olina.tech)
- [X — @olinatech](https://x.com/olinatech)
- [LinkedIn — Olina Tech](https://www.linkedin.com/company/olina-tech)
- [Reddit — u/olinatech](https://www.reddit.com/user/olinatech/)
- [GitHub — Olina-tech](https://github.com/Olina-tech)

---

<div align="center">

### Research deeply. Verify clearly. Build knowledge that lasts.

© 2026 Sirmint Technologies · Olina is a Sirmint Technologies product

</div>
