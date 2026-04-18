# Omega Project — Product Roadmap

> **Overview:** The Omega project is a dual-system autonomous AI platform comprised of **Omega 2.5** (the brain — a fully autonomous, local AI agent with a 4-layer cognitive stack) and **Omega CLI** (the developer agent — a TUI-driven coding assistant that delegates cognitive work to the brain via API). Both systems are zero-cloud, portable, and built for x64 Windows.

---

## Table of Contents

1. [Vision & Goals](#vision--goals)
2. [Current State (April 2026)](#current-state-april-2026)
3. [Phase 1 — Foundation Hardening](#phase-1--foundation-hardening-q2-2026)
4. [Phase 2 — CLI Rebuild & Brain Integration](#phase-2--cli-rebuild--brain-integration-q3-2026)
5. [Phase 3 — Capability Expansion](#phase-3--capability-expansion-q4-2026)
6. [Phase 4 — Distribution & Ecosystem](#phase-4--distribution--ecosystem-q1-2027)
7. [Long-Term Vision](#long-term-vision-2027)
8. [Architecture Reference](#architecture-reference)

---

## Vision & Goals

| Goal | Description |
|------|-------------|
| **Zero Cloud** | All inference runs locally — no data leaves the machine |
| **Portable** | Ships on a flash drive; runs on any x64 Windows machine |
| **Unified Brain** | CLI is a clean client of the Omega Brain, not a parallel system |
| **Cognitive Continuity** | Long-term memory persists across all sessions via Dewey filesystem |
| **Developer-First** | Omega CLI provides a best-in-class local AI coding experience |

---

## Current State (April 2026)

### Omega 2.5 — The Brain

- ✅ 4-layer cognitive stack (L1–L4) operational
- ✅ BrainLoop cycle: PERCEIVE → CLASSIFY → THINK → ACT
- ✅ Dewey memory filesystem (8 lobes, DME coordinate geometry)
- ✅ 7-module autonomic immune system (safety, dopamine, plasticity, etc.)
- ✅ Multi-modal: Voice (Whisper STT + Piper TTS), Vision (RetinaFace + ArcFace)
- ✅ HTTP Brain API on `:9200`, WebSocket on `:9210`
- ✅ 803 tests passing across 77 test files
- ✅ 20.5-second headless boot
- ⚠️ Boot time optimization needed
- ⚠️ MetaLayer / Deep Sleep Phase still being tuned

### Omega CLI — The Developer Agent

- ✅ Textual TUI interface operational
- ✅ 6 backend adapters (OpenAI, Azure, Anthropic, LM Studio, FLM/NPU, llama.cpp)
- ✅ 14 tool categories (~30 tools) with safety classifications
- ✅ Dewey memory integration (read from filesystem, write via Brain API)
- ✅ 3-tier autonomy system (READ_ONLY → SEMI_AUTO → FULL_AUTO)
- ✅ Auto-save sessions + `/resume`
- 🔄 **Active rebuild** per `2026-04-15-plumbing-rebuild-design.md` (69% code reduction in progress)
- ⚠️ Context management at rolling-window stage; Dewey long-term recall needs polish

---

## Phase 1 — Foundation Hardening (Q2 2026)

**Theme:** Stabilize both systems as a reliable base before expanding features.

### Omega 2.5

| Task | Priority | Status |
|------|----------|--------|
| Reduce boot time below 10 seconds | High | 🔄 In Progress |
| Tune MetaLayer scoring thresholds | High | 📋 Planned |
| Complete Deep Sleep Phase introspection | Medium | 📋 Planned |
| Expand test coverage to 95%+ | High | 📋 Planned |
| Document Brain API endpoints (OpenAPI spec) | High | 📋 Planned |
| Stabilize 97-tick epoch scheduler | Medium | 📋 Planned |
| Harden identity enforcement + safety guard | High | 📋 Planned |

### Omega CLI

| Task | Priority | Status |
|------|----------|--------|
| Complete plumbing rebuild (target ≤4,200 lines) | High | 🔄 In Progress |
| Full test suite for core engine + session | High | 📋 Planned |
| Stabilize Dewey write path (DEV lobe 700) | High | 📋 Planned |
| Harden auto-boot of llama-server | Medium | 📋 Planned |
| CLI trust system (`omega-cli trust`) polish | Medium | 📋 Planned |

### Milestones

- **M1.1** — Brain API fully documented with OpenAPI spec
- **M1.2** — Omega 2.5 boots in < 10 seconds
- **M1.3** — CLI rebuild complete; all existing tests green

---

## Phase 2 — CLI Rebuild & Brain Integration (Q3 2026)

**Theme:** Make the CLI a first-class, clean client of the Omega Brain.

### CLI as Brain Client

| Task | Priority | Status |
|------|----------|--------|
| CLI delegates all reasoning to Brain API (:9200) | High | 📋 Planned |
| Replace CLI-local context summarization with Dewey recall API | High | 📋 Planned |
| Real-time Brain status in CLI status bar (WebSocket :9210) | Medium | 📋 Planned |
| CLI auto-detects OmegaBrain volume + connects | Medium | ✅ Done |
| Unified memory writes: all lobes routable from CLI | High | 📋 Planned |
| Vision lobe (300) save/recall from CLI `vision.py` | Medium | 📋 Planned |

### Tool Enhancements

| Task | Priority | Status |
|------|----------|--------|
| `memory.py` — full lobe selector (not just DEV 700) | Medium | 📋 Planned |
| `project.py` — scaffold templates (Python, TS, Rust) | Medium | 📋 Planned |
| `test.py` — pytest coverage report integration | Low | 📋 Planned |
| `web.py` — structured extraction (tables, code blocks) | Medium | 📋 Planned |
| `git.py` — PR diff + review summary tool | Medium | 📋 Planned |

### Milestones

- **M2.1** — CLI reasoning fully delegated to Brain API
- **M2.2** — Real-time Brain health visible in CLI TUI
- **M2.3** — All 14 tool categories stable and documented

---

## Phase 3 — Capability Expansion (Q4 2026)

**Theme:** Unlock advanced cognitive and multi-modal features across both systems.

### Omega 2.5 — Advanced Cognition

| Task | Priority | Status |
|------|----------|--------|
| Loop B (cross-domain synthesis) production-ready | High | 📋 Planned |
| Learning Loop A reliability improvements | High | 📋 Planned |
| Add model slot: Code-specialized LLM (e.g., Qwen-Coder) | Medium | 📋 Planned |
| Improve face recognition accuracy (ArcFace pipeline) | Medium | 📋 Planned |
| Dewey lobe expansion: PROJECTS lobe (800) | Low | 📋 Planned |
| Temporal grounding improvements (date/time awareness) | Medium | 📋 Planned |

### Omega CLI — UX & Power Features

| Task | Priority | Status |
|------|----------|--------|
| Multi-file diff view in TUI | Medium | 📋 Planned |
| Background agent mode (autonomous task execution) | High | 📋 Planned |
| Plugin/extension API for community tools | Low | 📋 Planned |
| NPU backend (FLM) — stable & documented | High | 📋 Planned |
| Session branching (fork conversation + merge) | Low | 📋 Planned |
| `omega-cli doctor` diagnostics command | Medium | 📋 Planned |

### Milestones

- **M3.1** — Background agent mode working end-to-end
- **M3.2** — Loop B synthesis producing usable cross-domain insights
- **M3.3** — NPU (FLM) backend passing all integration tests

---

## Phase 4 — Distribution & Ecosystem (Q1 2027)

**Theme:** Make both systems easy to install, share, and extend.

| Task | Priority | Status |
|------|----------|--------|
| Flash-drive installer (one-click setup for x64 Windows) | High | 📋 Planned |
| Signed Windows binaries + auto-update mechanism | High | 📋 Planned |
| Public Brain API SDK (Python client library) | Medium | 📋 Planned |
| Community model repository (curated local models) | Medium | 📋 Planned |
| Web HUD polish: real-time cognition visualization | Medium | 📋 Planned |
| Multi-instance Brain support (run 2 brains simultaneously) | Low | 📋 Planned |
| Omega CLI: `pip install omega-cli` package | Medium | 📋 Planned |

### Milestones

- **M4.1** — Flash-drive release with installer wizard
- **M4.2** — Public Python SDK published to PyPI
- **M4.3** — `omega-cli` available as a standalone pip package

---

## Long-Term Vision (2027+)

| Idea | Description |
|------|-------------|
| **Multi-Agent Mesh** | Multiple Omega 2.5 instances collaborating over LAN |
| **Hardware Expansion** | Native AMD NPU inference (Ryzen AI) for sub-2B models |
| **Mobile Brain** | Omega 2.5 lite on ARM (Snapdragon X / Apple Silicon via WSL) |
| **Omega Studio** | Visual IDE for inspecting cognitive state, memory lobes, and reasoning traces |
| **Open Protocol** | Publish the Brain API as an open standard for third-party agents |

---

## Architecture Reference

```
┌─────────────────────────────────────────────────────────────┐
│                        Omega 2.5 (Brain)                    │
│                                                             │
│  L1 Sensory  ─►  L2 Cognitive  ─►  L3 Autonomic  ─►  L4   │
│  Voice/Vision     BrainLoop         Immune Sys.     Deep    │
│  Whisper/Piper    PERCEIVE→ACT      (7 modules)     Sleep   │
│                                                             │
│  Memory: Dewey Filesystem (lobes 000–1000, DME coords)     │
│  API: HTTP :9200  │  WebSocket :9210  │  llama.cpp :52625  │
└────────────────────────────┬────────────────────────────────┘
                             │ Brain API (HTTP + WS)
┌────────────────────────────▼────────────────────────────────┐
│                      Omega CLI (Developer Agent)            │
│                                                             │
│  TUI (Textual)  ─►  Core Engine  ─►  Tool Registry         │
│  Chat / Status      Session/Context   ~30 tools             │
│  Commands           Autonomy Tiers    files/search/git/...  │
│                                                             │
│  Backends: OpenAI │ Azure │ Anthropic │ LM Studio │ FLM    │
│  Memory: DeweyReader (fs) + DeweyWriter (Brain API)        │
└─────────────────────────────────────────────────────────────┘
```

---

## Status Legend

| Symbol | Meaning |
|--------|---------|
| ✅ | Complete |
| 🔄 | In Progress |
| 📋 | Planned |
| ⚠️ | Needs Attention |
| 🚫 | Blocked |

---

*Last updated: April 2026*
