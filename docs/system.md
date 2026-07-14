# AutomatosX system architecture

Aligned with the official product architecture infographic  
([HTML](../assets/AutomatosX_Infographic.html) · [PNG](../assets/AutomatosX_Infographic.png)).

The full system includes **public** products (open GitHub repositories) and **private** products (enterprise / closed-source components of the same architecture). Private products are part of AutomatosX; their source repositories are not linked here.

---

## Layered product architecture

### 1. User endpoints — application entry points

| Product | Role | Description | Availability |
|---------|------|-------------|--------------|
| **AX Studio** | General GenAI workspace | Enterprise knowledge + agentic workflows | Public — [ax-studio](https://github.com/defai-digital/ax-studio) |
| **AX Code** | AI coding & automation | IT / developer optimized agent runtime | Public — [ax-code](https://github.com/defai-digital/ax-code) |

These are the surfaces people open every day.

### 2. Governance layer — trust & policy enforcement

| Product | Role | Description | Availability |
|---------|------|-------------|--------------|
| **AX Trust** | Deterministic AI pipeline · core differentiator | Contract-based execution · guardrails + policy · full audit trail & explainability | Private — enterprise product |

Governance sits **between** users and infrastructure so execution can be constrained, audited, and reproduced.

### 3. AI infrastructure — serving · knowledge · inference

| Product | Role | Description | Availability |
|---------|------|-------------|--------------|
| **AX Serving** | Enterprise orchestration | Multi-node routing · heterogeneous compute · edge / offline deployment | Private — enterprise product |
| **AX Fabric** | Knowledge infrastructure | RAG + distillation · knowledge lifecycle · distilled reasoning layer | Private — enterprise product |
| **AX Engine** | Mac-native inference | Apple Silicon optimized · unified memory · large local models | Public — [ax-engine](https://github.com/defai-digital/ax-engine) |

---

## System data flow

Visual: [Infographic (HTML)](../assets/AutomatosX_Infographic.html) · [PNG](../assets/AutomatosX_Infographic.png)

| Hop | Product | Responsibility | Availability |
|-----|---------|----------------|--------------|
| User | **AX Studio** / **AX Code** | Intent via workspace or coding agents | Public |
| Governance | **AX Trust** | Contracts, guardrails, policy, audit hooks | Private |
| Routing | **AX Serving** | Route work across runtimes and nodes | Private |
| Inference | **AX Engine** | Local Mac inference (or external LLMs when allowed) | Public |
| Knowledge | **AX Fabric** | Knowledge retrieval, memory, lifecycle | Private |

Not every deployment enables every hop on day one. A minimal public stack is **AX Studio or AX Code → AX Engine**. Enterprise deployments add **AX Trust**, **AX Serving**, and **AX Fabric** for full governance, fleet orchestration, and private knowledge.

---

## Heterogeneous compute

AutomatosX is designed for **mixed hardware**, not a single cloud GPU SKU:

| Node class | Role |
|------------|------|
| **Mac Studio grid** | Control plane + light inference · Apple Silicon · unified memory |
| **Jetson Thor grid** | Heavy inference + CV · edge-deployable · air-gap ready |
| **DGX / cluster (future)** | Datacenter scale · architecture-agnostic extension |

**AX Engine** is the Mac-native inference product in this design. **AX Serving** is the private orchestration front door across heterogeneous nodes.

---

## Key differentiation (system level)

| | Thesis |
|---|--------|
| **A · Missing governance layer** | Market focus is often inference alone. AutomatosX adds governance + orchestration + reproducibility **above** LLMs (**AX Trust**, **AX Serving**). |
| **B · Sovereign / offline AI** | Air-gapped deployment; defence-ready patterns; Mac + Jetson hybrid; zero mandatory cloud API dependency. |
| **C · Deterministic vs probabilistic** | Contract-first execution (**AX Trust**) for enterprise reliability and auditability. |
| **D · Heterogeneous compute** | Control on Mac; heavy work on edge/grid; path to larger clusters (**AX Serving**). |

---

## Public repositories

Only these system roles publish open repositories for general use:

| System role | Product | Repository |
|-------------|---------|------------|
| User endpoint (workspace) | AX Studio | [github.com/defai-digital/ax-studio](https://github.com/defai-digital/ax-studio) |
| User endpoint (coding) | AX Code | [github.com/defai-digital/ax-code](https://github.com/defai-digital/ax-code) |
| Mac inference | AX Engine | [github.com/defai-digital/ax-engine](https://github.com/defai-digital/ax-engine) |

**AX Trust**, **AX Serving**, and **AX Fabric** are private products in the same system. Contact DEFAI for enterprise access — no public source links are published in this documentation.

---

## Related docs

- [Introduction](introduction.md)  
- [Product directory](products.md)  
- [Getting started](getting-started.md)  
