<!-- ────────────────────────────  HEADER  ──────────────────────────── -->

<p align="center">
  <img src="assets/Logo.svg" alt="InfraPolus" width="100%"/>
</p>

<h1 align="center">I N F R A P O L U S</h1>

<h2 align="center">
  Building the intelligence infrastructure for autonomous systems.
</h2>

<p align="center">
  <b>Secure. Persistent. Verifiable. Agentic.</b>
</p>

<p align="center">
  <code>&nbsp;AGENTIC&nbsp;INTELLIGENCE&nbsp;</code>
  <code>&nbsp;KNOWLEDGE&nbsp;ENGINEERING&nbsp;</code>
  <code>&nbsp;HYBRID&nbsp;RETRIEVAL&nbsp;</code>
  <code>&nbsp;AI&nbsp;SECURITY&nbsp;</code>
  <code>&nbsp;OFFLINE&nbsp;FIRST&nbsp;</code>
</p>

---

<br/>

<h2 align="center">The next generation of AI systems will not be built by models alone.</h2>

<br/>

Large language models changed how machines process information.

But **intelligence without memory**, **reasoning without verification**, and **autonomy without control** are not enough.

The future belongs to systems capable of:

- understanding complex environments
- accumulating knowledge over time
- making reliable decisions
- executing actions safely
- improving through experience

InfraPolus is building the foundational architecture required for this next generation of autonomous intelligence.

<br/>

---

<br/>

<h2 align="center">Beyond AI assistants. Toward intelligent infrastructure.</h2>

<br/>

Current AI systems are limited by fragmented context, stateless interactions and unreliable execution.

InfraPolus explores a different paradigm:

<h3 align="center">AI systems as engineered entities.</h3>

<p align="center">Systems that combine</p>

```
        KNOWLEDGE  +  REASONING  +  VERIFICATION  +  SECURITY  +  AUTONOMOUS EXECUTION
```

<p align="center">to create reliable agentic architectures.</p>

<br/>

---

<br/>

# Core Technologies

### Agentic Intelligence

Designing autonomous systems capable of planning, reasoning and executing complex objectives — within measured bounds.

Research areas:

- bounded agentic loops (task-level budgets, not per-turn limits)
- tool orchestration and execution control
- uncertainty tracking and active research agendas
- agent evaluation

> Deliberation and parallel LLM subagents were evaluated and **rejected with
> measured evidence** (net quality damage on a 9B local model, plus a VRAM
> budget that cannot host two models). The rejection is documented, not
> hidden: see DEC-009 and RES-006 in IPA's engineering memory.

Implemented in: [IPA — agent core & cognitive layer](https://github.com/ValenByteTar/IPA)

<br/>

### Knowledge Engineering

**Intelligence requires memory.**

InfraPolus develops knowledge architectures that allow AI systems to accumulate, organize and retrieve experience.

Current focus:

- Hybrid Retrieval Systems (semantic + lexical + sparse, rank-fused)
- re-ranking with cross-encoders
- provenance-preserving ingestion pipelines
- context optimization
- persistent engineering memory

Implemented in: [IPA](https://github.com/ValenByteTar/IPA) — retrieval evaluation in `knowledge/benchmarks/` (BM-002, BM-005), rerank stage-2 in `knowledge/experiments/EXP-007` (+20.5pp recall@1).

<br/>

### Engineering Knowledge Systems (EKS)

Software engineering knowledge is usually lost between projects, conversations and teams.

EKS transforms engineering experience into a structured intelligence layer, capturing:

- architectural decisions
- experiments
- benchmarks
- failures (postmortems)
- patterns
- technical research

Every accepted record requires verifiable evidence paths. Records declare which paths they govern (`affects`), and coding agents receive those records injected before touching the code they govern.

The objective:

> Build AI systems that do not only generate code, but understand the engineering knowledge behind it.

Live at: [`IPA/knowledge/`](https://github.com/ValenByteTar/IPA/tree/main/knowledge) — 45+ records, validated in CI.

<br/>

### Cybersecurity for Autonomous Systems

Autonomous systems introduce a new security frontier.

InfraPolus investigates:

- agent security
- knowledge integrity (provenance-preserving pipelines)
- execution isolation and resource arbitration (file leases with heartbeat, work permits for parallel agent sessions)
- secure AI infrastructure — local-first by design: data never leaves the machine

Implemented in: [IPA — work permits & leases](https://github.com/ValenByteTar/IPA/tree/main/tools) · [PAT-007](https://github.com/ValenByteTar/IPA/tree/main/knowledge/patterns)

<br/>

---

<br/>

# Architecture Philosophy

<h3 align="center">Intelligence needs foundations.</h3>

<p align="center">Better models alone will not create reliable autonomous systems.</p>

<p align="center">The next evolution requires:</p>

<br/>

| | | | |
|---|---|---|---|
| **Persistent Knowledge**<br>Systems must remember. | **Verification Layers**<br>Systems must prove. | **Controlled Execution**<br>Systems must act safely. | **Engineering Discipline**<br>Systems must be designed, measured and improved. |

<br/>

---

<br/>

# Current Platform: IPA

IPA is a local-first knowledge acquisition and materialization platform for agents: it turns heterogeneous sources into canonical, provenance-preserving knowledge, and serves it to agents through derived lexical, vector and enriched views.

It runs entirely on consumer hardware — a laptop with a 6 GB GPU. No cloud. No paid APIs. Data never leaves the machine.

Current scale:

```
300K+    indexed chunks (BM25 + LanceDB, synchronized)
4,500+   documents under management
1,100+   tests in CI
40+      engineering records (decisions, benchmarks, postmortems)
local    full inference pipeline — no external APIs
```

→ [ValenByteTar/IPA](https://github.com/ValenByteTar/IPA) — clone it, run the tests, read the postmortems. Everything stated here is verifiable.

<br/>

### The lineage

Three generations, each superseding the last — every supersession documented:

| Generation | Repository | Status |
|---|---|---|
| v1 — Hybrid RAG | [SistemaRAGHybrid](https://github.com/ValenByteTar/SistemaRAGHybrid) | Complete. Superseded by AgenticRAG. |
| v2 — Agentic RAG | [AgenticRAG](https://github.com/ValenByteTar/AgenticRAG) | Feature-complete, not polished. Superseded by IPA after structural problems it surfaced. |
| v3 — Platform | [IPA](https://github.com/ValenByteTar/IPA) | Current. Local-first knowledge platform for agents. |

The evaluation work that decided IPA's local engine lives in [small-model-deliberation](https://github.com/ValenByteTar/small-model-deliberation) (58 runs, controlled comparison).

<br/>

---

<br/>

<h1 align="center">The Mission</h1>

<h3 align="center">
  Build the infrastructure layer that allows artificial intelligence systems<br/>
  to evolve from assistants into reliable autonomous entities.
</h3>

<br/>

---

<br/>

# Roadmap

**Foundation Layer** — shipped in [SistemaRAGHybrid](https://github.com/ValenByteTar/SistemaRAGHybrid) and [AgenticRAG](https://github.com/ValenByteTar/AgenticRAG)

```
✓  Retrieval infrastructure
✓  Local AI inference
✓  Evaluation framework
✓  Knowledge storage architecture
```

**Intelligence Layer** — shipped in [IPA](https://github.com/ValenByteTar/IPA)

```
✓  Engineering Knowledge System (45+ records, CI-validated)
✓  Agent context enrichment
✓  Decision-aware workflows
```

**Autonomous Systems Layer** — in progress

```
▸  Self-improving engineering workflows
▸  Secure autonomous agents
▸  Distributed intelligence architectures
```

<br/>

---

<br/>

<h1 align="center">I N F R A P O L U S</h1>

<h3 align="center">Secure intelligence for the next generation of agentic systems.</h3>

<br/>

