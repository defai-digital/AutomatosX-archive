# Getting started with AutomatosX

This guide starts from the **three public products** that introduce the AutomatosX system. Always follow install steps in each product’s own README — versions and commands change.

---

## Choose an entry point

| You want… | Open this repository |
|-----------|----------------------|
| Desktop GenAI workspace | [defai-digital/ax-studio](https://github.com/defai-digital/ax-studio) |
| Coding agents on real repos | [defai-digital/ax-code](https://github.com/defai-digital/ax-code) |
| Local models on Apple Silicon | [defai-digital/ax-engine](https://github.com/defai-digital/ax-engine) |

**Recommended first system:** Studio **or** Code + Engine on a Mac.

```text
Install AX Engine → serve a model
        ↓
Install AX Studio and/or AX Code
        ↓
Point the client at the Engine endpoint (or use cloud providers while you evaluate)
```

---

## Path A — AX Studio

1. Open **[github.com/defai-digital/ax-studio](https://github.com/defai-digital/ax-studio)**  
2. Follow the README for desktop install (including Homebrew taps if listed)  
3. Connect a cloud provider **or** a local OpenAI-compatible base URL  
4. Optionally add MCP servers for tools  

Studio is the **general workspace** entry to AutomatosX.

---

## Path B — AX Code

1. Open **[github.com/defai-digital/ax-code](https://github.com/defai-digital/ax-code)**  
2. Install per README (CLI / TUI / desktop as available)  
3. Open a repository and start a session  
4. Configure isolation / permissions for the task  
5. Attach MCP tools or skills as needed  

Code is the **developer / automation** entry to AutomatosX.

---

## Path C — AX Engine (local inference)

1. Open **[github.com/defai-digital/ax-engine](https://github.com/defai-digital/ax-engine)**  
2. Install the engine (wheel / Homebrew as documented)  
3. Download or prepare a supported model  
4. Run the documented `serve` (or equivalent) command  
5. Configure Studio or Code to use that OpenAI-compatible endpoint  

Engine is the **Mac inference** pillar of AutomatosX infrastructure.

---

## Minimal sovereign-leaning stack

For a laptop / Mac Studio style evaluation without cloud dependency:

| Step | Component | Purpose | Availability |
|------|-----------|---------|--------------|
| 1 | [AX Engine](https://github.com/defai-digital/ax-engine) | Local inference | Public |
| 2 | [AX Studio](https://github.com/defai-digital/ax-studio) and/or [AX Code](https://github.com/defai-digital/ax-code) | User endpoints | Public |
| 3 | **AX Trust**, **AX Serving**, **AX Fabric** | Governance, fleet orchestration, private knowledge | Private enterprise products |

That path matches the architecture story: **users → governance → infrastructure**, starting with the public products. AX Trust, AX Serving, and AX Fabric remain first-class parts of the system; contact DEFAI for enterprise access (no public source links in these docs).

---

## What not to expect from *this* repository

- No `npm install` application monorepo  
- No substitute for product release notes  
- No public source links for private products (AX Trust, AX Serving, AX Fabric)  

This repo **introduces the full system** and only publishes GitHub links for the public products:

- https://github.com/defai-digital/ax-studio  
- https://github.com/defai-digital/ax-code  
- https://github.com/defai-digital/ax-engine  

---

## Next reading

- [Introduction](introduction.md)  
- [System architecture](system.md)  
- [Product directory](products.md)  
- Infographic: [HTML](../assets/AutomatosX_Infographic.html) · [PNG](../assets/AutomatosX_Infographic.png)  
