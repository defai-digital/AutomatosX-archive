# What is AutomatosX?

AutomatosX is a **sovereign AI orchestration and governance platform**. It is the system layer positioned **above inference engines** — application entry points, trust/policy, routing, knowledge, and local inference — built for enterprise, government, and defence-sensitive environments.

This documentation repository explains the **system**. Implementation lives in product repositories, especially:

- [AX Studio](https://github.com/defai-digital/ax-studio) — general GenAI workspace  
- [AX Code](https://github.com/defai-digital/ax-code) — AI coding & automation  
- [AX Engine](https://github.com/defai-digital/ax-engine) — Mac-native inference  

---

## Positioning

| Badge | Meaning |
|-------|---------|
| **Contract-first · Deterministic AI** | Pipelines and policies defined as contracts; reproducible execution |
| **Offline / air-gapped ready** | Operable without cloud dependency when required |
| **Governance above inference** | Not only “run a model” — control, audit, and orchestrate how AI is used |

---

## Four pillars

1. **Verifiable AI** — every decision is traceable, inspectable, and can be cryptographically anchored  
2. **Reproducible pipelines** — same input → same output under contract-based execution  
3. **Full audit trail** — explainability across reasoning steps and data flows  
4. **Sovereign / offline deployment** — air-gapped capable; true data sovereignty for sensitive operations  

---

## How people enter the system

| Entry product | Analogy (for orientation) | Audience |
|---------------|---------------------------|----------|
| **[AX Studio](https://github.com/defai-digital/ax-studio)** | General GenAI workspace (ChatGPT / Claude–class UX, enterprise-shaped) | Knowledge work, agentic workflows |
| **[AX Code](https://github.com/defai-digital/ax-code)** | AI coding runtime (Claude Code–class, enterprise-shaped) | Developers / IT automation |

Both sit on the **user endpoints** layer of the product architecture. Underneath them, the full system applies:

| Layer | Products | Availability |
|-------|----------|--------------|
| Governance | **AX Trust** | Private enterprise product |
| Routing / orchestration | **AX Serving** | Private enterprise product |
| Knowledge | **AX Fabric** | Private enterprise product |
| Local inference | **[AX Engine](https://github.com/defai-digital/ax-engine)** | Public |

Private products are part of the AutomatosX system architecture; their source repositories are not linked in this documentation.

---

## What problem it solves

Most of the market optimizes **inference** (faster engines, more GPUs). AutomatosX addresses what regulated and sovereign buyers still lack:

- **Governance + orchestration + reproducibility** above LLMs  
- **Offline / edge** deployment without mandatory cloud APIs  
- **Deterministic, contract-first** paths where pure probabilistic chat is not enough  
- **Heterogeneous compute** (Mac control plane + edge/heavy inference grids)  

---

## Who it is for

- Enterprises that need auditability and policy around AI use  
- Government and defence programmes that require air-gapped or sovereign deployments  
- Engineering teams that want coding agents under control (AX Code)  
- Teams running serious local models on Apple Silicon (AX Engine)  
- Organizations that want a coherent **system**, not a pile of unrelated chat tools  

---

## What this repo is / is not

| This repo | Not this repo |
|-----------|----------------|
| System introduction and architecture narrative | Source code for Studio / Code / Engine |
| Product map and GitHub directory | Install binaries or release artifacts |
| Infographic and orientation docs | Per-product API reference (see each product README) |

Continue with **[System architecture](system.md)** or **[Getting started](getting-started.md)**.
