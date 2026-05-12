<div align="center">

# agentic-patterns-library

![Patterns](https://img.shields.io/badge/patterns-50%2B-blue?style=flat)
![Source](https://img.shields.io/badge/source-nibzard%2Fawesome--agentic--patterns-lightgrey?style=flat)
![MAE](https://img.shields.io/badge/MAE-integrated-green?style=flat)
![Models](https://img.shields.io/badge/LLMs-Claude%20%7C%20Groq%20%7C%20Gemini-orange?style=flat)

**50+ production-grade agentic AI patterns — curated, categorized, DigiMinds-wired.**
ReAct, RAG, multi-agent orchestration, tool use, feedback loops, security, and more.

</div>

---

## Pattern Categories

| Category | Description | Patterns |
|---|---|---|
| **Orchestration & Control** | Agent loops, task decomposition, coordinator patterns | 8 |
| **Context & Memory** | RAG, vector stores, session memory, long-context | 7 |
| **Feedback Loops** | Self-critique, reflection, iterative refinement | 6 |
| **Learning & Adaptation** | Few-shot, fine-tuning signals, preference learning | 5 |
| **Reliability & Eval** | Guardrails, evals, fallback chains | 6 |
| **Security & Safety** | Injection defense, permission gates, sandboxing | 5 |
| **Tool Use & Environment** | MCP tools, API calls, code execution, browser | 8 |
| **UX & Collaboration** | Human-in-the-loop, approval flows, streaming | 5 |

## 🔥 Hot — Most Used Patterns

| Pattern | Type | Use case |
|---|---|---|
| **ReAct** | Orchestration | Reasoning + acting loop — foundation for most agents |
| **RAG** | Context & Memory | Retrieval-augmented generation — knowledge injection |
| **Multi-Agent Swarm** | Orchestration | Parallel specialist agents + synthesis |
| **Self-Critique** | Feedback | Agent reviews own output before returning |
| **Tool-Use Router** | Tool Use | Selects best tool/API for each sub-task |
| **OODA Loop** | Orchestration | Observe-Orient-Decide-Act rapid decision cycle |
| **Critic-Optimizer** | Feedback | Critic agent scores → Optimizer agent improves |
| **Guardrail Gate** | Reliability | Pre/post validation before executing risky actions |

## DigiMinds Integration

```bash
# MAE uses these patterns internally:
mae run "goal"          # ReAct + Multi-Agent Swarm + Critic-Optimizer
tcc blast "t1" "t2"     # Parallel Tool-Use + RAG per sub-task
llm-burst "prompt"      # 15-model burst → Judge pattern

# Pattern files location (after install):
~/installed-repos/awesome-agentic-patterns/patterns/
```

## Quick Install

```bash
git clone https://github.com/nibzard/awesome-agentic-patterns ~/installed-repos/awesome-agentic-patterns
cd ~/installed-repos/awesome-agentic-patterns
npm install
npm run dev   # Serve locally at http://localhost:4321
```

## Pattern File Format

```yaml
---
title: ReAct Pattern
status: production
category: Orchestration & Control
tags: [reasoning, tool-use, loop, foundational]
---
## Problem
Agent needs to reason AND act without losing context between steps.

## Solution
Interleave Thought → Action → Observation cycles until goal is reached.

## How to use it
...
```

## ■ tip

> Each pattern in `patterns/` directory has a YAML front-matter + structured Markdown doc.
> Run `npm run dev` to get a searchable web UI at localhost:4321.

---

## ☠️ AGENCIES / AI BUILDERS

**DigiMinds Global** uses these patterns as the architectural blueprint for MAE (Master Automation Engine),
TCC (Task Command Center), and all 210 specialist agents.

Pattern → Agent wiring: `~/.claude/tcc-routes/routes.json`

---

*Part of [hmzainjamil/claude-ai-system](https://github.com/hmzainjamil/claude-ai-system)*
