# Product directory

AutomatosX is a **system** of six products across three layers. Three are public open-source entry points; three are private enterprise products in the same architecture.

---

## Public products

These repositories are the open entry points for the AutomatosX system.

### AX Studio

| | |
|---|---|
| **Layer** | User endpoints |
| **Role** | General GenAI workspace |
| **Summary** | Enterprise knowledge + agentic workflows — the ChatGPT / Claude–class surface for organizations |
| **Availability** | Public |
| **Repository** | **[github.com/defai-digital/ax-studio](https://github.com/defai-digital/ax-studio)** |

Local-first desktop AI workspace: multi-provider chat, MCP tools, memory, artifacts, optional local models via OpenAI-compatible endpoints (including AX Engine).

### AX Code

| | |
|---|---|
| **Layer** | User endpoints |
| **Role** | AI coding & automation |
| **Summary** | IT / developer optimized agent runtime — Claude Code–class capability for enterprise repos |
| **Availability** | Public |
| **Repository** | **[github.com/defai-digital/ax-code](https://github.com/defai-digital/ax-code)** |

Local-first coding agents with durable sessions, sandbox isolation, MCP/skills, CLI/TUI/SDK, and production-shaped controls.

### AX Engine

| | |
|---|---|
| **Layer** | AI infrastructure |
| **Role** | Mac-native inference |
| **Summary** | Apple Silicon optimized runtime · unified memory · large local model performance |
| **Availability** | Public |
| **Repository** | **[github.com/defai-digital/ax-engine](https://github.com/defai-digital/ax-engine)** |

Mac-first LLM inference: model prepare/serve, OpenAI-compatible local endpoints, direct support for key model families. Point Studio or Code at Engine for offline-capable inference.

---

## Private products

These are **full members** of the AutomatosX system (see the infographic). Source repositories are private; they are not linked in this documentation. Enterprise access is through DEFAI.

### AX Trust

| | |
|---|---|
| **Layer** | Governance |
| **Role** | Deterministic AI pipeline · core differentiator |
| **Summary** | Contract-based execution · guardrails + policy enforcement · full audit trail & explainability |
| **Availability** | Private — enterprise product |

Sits between user endpoints and infrastructure so AI work can be constrained, audited, and reproduced.

### AX Serving

| | |
|---|---|
| **Layer** | AI infrastructure |
| **Role** | Enterprise orchestration |
| **Summary** | Multi-node routing · heterogeneous compute · edge / offline deployment |
| **Availability** | Private — enterprise product |

Fleet control plane over runtimes (including AX Engine and other certified inference backends).

### AX Fabric

| | |
|---|---|
| **Layer** | AI infrastructure |
| **Role** | Knowledge infrastructure |
| **Summary** | RAG + distillation · knowledge lifecycle management · distilled reasoning layer |
| **Availability** | Private — enterprise product |

Private knowledge backend for governed retrieval, memory, and semantic lifecycle.

---

## Architecture map (all products)

| Layer | Product | Role | Availability |
|-------|---------|------|--------------|
| User endpoints | **AX Studio** | General GenAI workspace | Public — [ax-studio](https://github.com/defai-digital/ax-studio) |
| User endpoints | **AX Code** | AI coding & automation | Public — [ax-code](https://github.com/defai-digital/ax-code) |
| Governance | **AX Trust** | Deterministic AI pipeline · contracts, guardrails, audit | Private |
| AI infrastructure | **AX Serving** | Enterprise orchestration · multi-node routing · edge/offline | Private |
| AI infrastructure | **AX Fabric** | Knowledge infrastructure · RAG + distillation · lifecycle | Private |
| AI infrastructure | **AX Engine** | Mac-native inference | Public — [ax-engine](https://github.com/defai-digital/ax-engine) |

---

## How they connect

See the system visual for layers and data flow:

- [Infographic (HTML)](../assets/AutomatosX_Infographic.html)
- [Infographic (PNG)](../assets/AutomatosX_Infographic.png)
- [System architecture](system.md)

---

## Next

- [System architecture](system.md)  
- [Getting started](getting-started.md)  
