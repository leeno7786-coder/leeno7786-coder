<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0b1220,45:111827,100:0ea5e9&height=220&section=header&text=Omega%20AI%20LLC&fontSize=52&fontColor=ffffff&fontAlignY=40&desc=Sovereign%20intelligence%20—%20local-first,%20memory-first,%20bounded%20autonomy&descSize=16" alt="Omega AI LLC banner">
</p>

# Omega AI LLC

**Noah Lee** — founder · Louisiana  
Local-first AI systems for cloud, edge, and on-device deployments. The company builds the architecture; this page is the index for the work.

[omega2ai.com](https://www.omega2ai.com) · [noahlee@omega2ai.com](mailto:noahlee@omega2ai.com) · [GitHub](https://github.com/leeno7786-coder)

We take on metacognitive / agentic systems, custom AI runtimes, local and edge inference, web and Android applications, and Linux / hardware integration. If the problem is “the model is not the product,” that is the work.

---

## What we build

Omega is a **portable, memory-first autonomous cognitive substrate**: bounded autonomy, offline learning, reversible evolution. Not a chat wrapper. A cognition loop with a memory cortex, a local runtime, and swappable hands (tools, browsers, MCP providers, CLIs).

| Layer | Job |
| --- | --- |
| **Cognition** | Episode-scoped cascade. Most stages are deterministic. Only a few layers run a model. |
| **Memory** | Single cortex: gated writes, promotion, contradiction handling, taxonomy, verified recall. |
| **Runtime** | Local inference contract (portable / NPU / Windows + Linux). The brain does not own the metal. |
| **Surfaces** | MCP servers, coding agents, voice, embedded browser, product UIs. |

**How we decide if the architecture is right:** if it cannot run offline on a laptop, the product is wrong.

---

## Flagship — Omega 3.0

Private product. Python 3.13+. Modular packages. Patent-aware commercial work.

A single **episode** is the carrier. Walk order:

```
Pressure → Global A → Meta A → AUTO → Meta B → Global B → Omega → DeepSleep
```

- **Pressure** ignites the loop; it does not replace it.
- **AUTO** and **Omega** are the only model-running layers.
- **Meta B** and **Global B** are deterministic (no inference).
- **DeepSleep** closes the episode, resets pressure, reseeds, and consolidates memory.
- **Guardian** classifies responses and gates memory writes.
- **Autonomic** layer tracks plasticity, strength, stress, and temporal grounding.
- Inference stays local via **omega-portable-lite** and the **omega-runtime** Windows gateway against the same brain contract.

Public highlights and demos: [omega2ai.com](https://www.omega2ai.com). Technical access, partnership, or services: [noahlee@omega2ai.com](mailto:noahlee@omega2ai.com).

### Lineage — Omega 2.5

The prior local-first agent (AMD Lemonade Developer Challenge). On-device path on Ryzen AI / Radeon iGPU / XDNA2 NPU: Lemonade Server, Gemma 4 E2B (Qwen 3.5 4B fallback), local voice, embedded Playwright Chromium + Manifest V3 extension, Dewey 3D memory cortex, SetFit routing. That stack is what Omega 3.0 generalized into a substrate.

---

## Public work

### NanoAgent

Ultra-lightweight CLI/TUI coding agent for **tiny local models** (2B–8B, especially Qwen 2.5/3.5). Also speaks OpenAI, Anthropic, OpenRouter, and DashScope.

[`leeno7786-coder/nanoagent`](https://github.com/leeno7786-coder/nanoagent) · `@omega3_0/nanoagent` 2.1.5 · MIT

- OpenTUI dashboard — streaming chat, tool diffs, todos, skills
- Dual-level config, permission modes, workspace sandbox, secret redaction
- MCP (stdio + HTTP), skills system, memory graph
- Remote sub-agents; headless `run` / `doctor` / `models` for scripts and CI
- Native packages: Linux `.deb` and Windows zip (bundled Node 20)

Actively developed; treat current releases as WIP. Issues and PRs welcome.

### Company site

[`omega-site`](https://github.com/leeno7786-coder/omega-site) — React 19, TypeScript, Vite, Tailwind, shadcn/ui, Three.js, GSAP. Live at [omega2ai.com](https://www.omega2ai.com).

### Productized web

**DevCard AI** — AI portfolio generator. Next.js 16, Clerk, Stripe. [www.omega-dev.uk](https://www.omega-dev.uk)

---

## Platform & enablement

Work that sits next to the brain, not inside it:

- **Omega Memory MCP** — standalone local memory server (Dewey taxonomy, graph projections, verified recall). One install wires Cursor, Claude Desktop/Code, VS Code, Gemini, OpenCode, Copilot CLI, Codex, and other MCP hosts.
- **Omega Google Workspace MCP** — first-party stdio provider behind a hard architecture rail: provider code may only import `mcp_platform` contracts. Tests enforce the boundary.
- **omega-runtime** — greenfield Windows AI runtime gateway for the Omega 3.0 brain contract (Python, PowerShell, C++).
- **Ryzen AI / NPU** — portable AMD runtime and Linux enablement (Python + C++).

---

## Knowledge we actually ship

This is not a keyword list. It is what the repos contain.

**Languages & systems** — Python 3.12–3.13 (cognition, memory, MCP, runtimes); TypeScript / JavaScript (agents, site, product apps); PowerShell and Bash (installers, Windows + Linux packaging); C++ where the runtime meets the metal.

**AI systems** — metacognitive loops, episode orchestration, long-horizon memory, local LLM serving, tiny-model tool calling, GGUF on-device models, embeddings and classifiers (SetFit, Harrier).

**Agent platforms** — MCP (stdio/HTTP, multi-host installers), skills, CLI/TUI agents, browser agents (Playwright + MV3), voice loops.

**Edge & hardware** — AMD Lemonade, Ryzen AI / NPU, GPU lease / hotswap control, local-only inference contracts, Debian and portable Windows packaging.

**Product** — Next.js, React, Vite, Tailwind, Clerk, Stripe, Netlify, GitHub Actions / Pages.

**Engineering rails** — architecture tests as contracts, provider/brain boundaries, installers that wire real agent hosts, reversible / auditable autonomy.

### Design rules

1. **The brain is not the hands.** Cognition decides. Executors, browsers, MCP providers, and runtimes are limbs behind contracts.
2. **Most of the loop should not call a model.** Deterministic packs, gates, and journals keep autonomy inspectable.
3. **Memory is infrastructure.** Taxonomy, promotion gates, and verified recall — not a vector dump in the prompt.
4. **Local-first is a constraint.** Offline on a laptop NPU, or the architecture is unfinished.

---

## Engage

| Need | Where |
| --- | --- |
| Demos, Omega 3.0 access, custom runtime / agent / hardware work | [noahlee@omega2ai.com](mailto:noahlee@omega2ai.com) · [omega2ai.com](https://www.omega2ai.com) |
| Use or contribute to the public coding agent | [nanoagent](https://github.com/leeno7786-coder/nanoagent) |
| Company site source | [omega-site](https://github.com/leeno7786-coder/omega-site) |

Public contributions are accepted on NanoAgent. Collaboration on Omega 3.0 is by access and partnership.

---

## License

This overview repository is MIT. NanoAgent is MIT. Omega 3.0 remains a private product.

© 2026 Omega AI LLC
