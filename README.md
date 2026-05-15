# agentic-patterns-library
50+ production AI agent patterns — ReAct, RAG, multi-agent, tool-use, orchestration blueprints

![Python](https://img.shields.io/badge/Python-3.11+-3776AB?style=flat&labelColor=555&logo=python)
![Claude](https://img.shields.io/badge/Claude-Code-cc785c?style=flat&labelColor=555)
![LangChain](https://img.shields.io/badge/LangChain-Patterns-green?style=flat&labelColor=555)
![Patterns](https://img.shields.io/badge/Patterns-50+-blue?style=flat&labelColor=555)
![Status](https://img.shields.io/badge/Status-Active-brightgreen?style=flat&labelColor=555)

[Concepts](#-concepts) · [How It Works](#️-how-it-works) · [Patterns](#-pattern-library) · [Install](#-install) · [Tips](#-tips-and-tricks-10) · [Startups](#️-startups--businesses)

---

## 🧠 CONCEPTS

| Feature | Location | Description |
|---------|----------|-------------|
| [**ReAct Pattern**](patterns/react/) | `patterns/react/` | Reasoning + Acting loop — think, act, observe, repeat |
| [**RAG Pattern**](patterns/rag/) | `patterns/rag/` | Retrieval-Augmented Generation — ground LLM in real data |
| [**Multi-Agent**](patterns/multi-agent/) | `patterns/multi-agent/` | Orchestrator + specialist agents — parallel task execution |
| [**Tool Use**](patterns/tool-use/) | `patterns/tool-use/` | Function calling, MCP tools, API integration |
| [**Memory Systems**](patterns/memory/) | `patterns/memory/` | Short-term, long-term, episodic, semantic memory |
| [**Self-Improvement**](patterns/self-improve/) | `patterns/self-improve/` | DSPy, GEPA, auto-prompt optimization |

### 🔥 Hot

| Feature | Location | Description |
|---------|----------|-------------|
| [**AGENT.md Standard**](AGENT.md) | `AGENT.md` | Standardized agent contract — capabilities, tools, constraints |
| [**Orchestration Blueprints**](patterns/orchestration/) | `patterns/orchestration/` | MAE, TCC, Paperclip-style agent orchestration patterns |
| [**Production-ready**](patterns/) | All patterns | Battle-tested in DigiMinds agency ops — not toy examples |

---

## ⚙️ HOW IT WORKS

Each pattern is a self-contained directory:
```
patterns/react/
  ├── pattern.md          — explanation + when to use
  ├── implementation.py   — working Python code
  ├── example.py          — real-world example
  └── tests/              — unit tests
```

**Pattern selection guide:**
- Single task, tool access → **ReAct**
- Need external knowledge → **RAG**
- Complex goal, parallelizable → **Multi-Agent**
- Structured output → **Tool Use / Function Calling**
- Long-running context → **Memory Systems**

---

## 📚 PATTERN LIBRARY

| Category | Patterns | Key Use Case |
|---|---|---|
| **Reasoning** | ReAct, Chain-of-Thought, Tree-of-Thought, Self-Consistency | Complex problem solving |
| **Retrieval** | RAG, Hybrid Search, Re-ranking, Contextual Compression | Knowledge grounding |
| **Multi-Agent** | Orchestrator-Worker, Peer-to-Peer, Hierarchical, Swarm | Parallel execution |
| **Memory** | Buffer, Summary, Vector, Entity, Episodic | Context persistence |
| **Tool Use** | Function Calling, MCP, API Chains, Browser Control | External actions |
| **Optimization** | DSPy, GEPA, Constitutional AI, Self-Critique | Auto-improvement |
| **Safety** | Guardrails, Input Validation, Output Filtering | Production safety |
| **Orchestration** | MAE-style, TCC-style, Paperclip-style, DAG | System design |

---

## 🚀 INSTALL

```bash
git clone https://github.com/hmzainjamil/agentic-patterns-library
cd agentic-patterns-library
pip install -r requirements.txt
# Browse patterns/
python3 patterns/react/example.py
```

---

## 💡 TIPS AND TRICKS (10)

[selection](#tips-selection) · [react](#tips-react) · [rag](#tips-rag) · [multiagent](#tips-multiagent)

<a id="tips-selection"></a>■ **Pattern Selection (3)**

| Tip | Source |
|-----|--------|
| Start with ReAct — it handles 80% of agentic tasks with minimal complexity | [HMZ](https://github.com/hmzainjamil) |
| Multi-agent only when tasks are truly parallelizable — overhead kills sequential tasks | [DigiMinds](https://github.com/hmzainjamil) |
| Memory pattern before RAG — check if simple context window solves the problem first | [HMZ](https://github.com/hmzainjamil) |

<a id="tips-react"></a>■ **ReAct (3)**

| Tip | Source |
|-----|--------|
| Limit ReAct to 10 iterations max — add hard stop to prevent infinite loops | [HMZ](https://github.com/hmzainjamil) |
| Log every Thought/Action/Observation — debugging ReAct without logs is impossible | [DigiMinds](https://github.com/hmzainjamil) |
| Groq for ReAct loops — 200tok/s means faster iterations, better UX | [HMZ](https://github.com/hmzainjamil) |

<a id="tips-rag"></a>■ **RAG (2)**

| Tip | Source |
|-----|--------|
| Hybrid search (vector + BM25) beats pure vector search on factual recall by ~20% | [HMZ](https://github.com/hmzainjamil) |
| Re-rank retrieved docs before sending to LLM — cuts context by 60%, improves answers | [DigiMinds](https://github.com/hmzainjamil) |

<a id="tips-multiagent"></a>■ **Multi-Agent (2)**

| Tip | Source |
|-----|--------|
| Orchestrator should be Groq (fast decomposition) — workers can be cheaper models | [HMZ](https://github.com/hmzainjamil) |
| Use TCC pattern for agent queuing — persistent queue survives agent crashes | [DigiMinds](https://github.com/hmzainjamil) |

---

## ☠️ STARTUPS / BUSINESSES

| This Repo / Feature | Replaced |
|-|-|
| **ReAct implementation** | [LangChain Agents](https://langchain.com), [LlamaIndex](https://llamaindex.ai) |
| **RAG patterns** | [Pinecone](https://pinecone.io), [Weaviate](https://weaviate.io), [Chroma](https://trychroma.com) |
| **Multi-agent blueprints** | [AutoGen](https://microsoft.github.io/autogen/), [CrewAI](https://crewai.com), [AgentGPT](https://agentgpt.reworkd.ai) |
| **Self-improvement patterns** | [DSPy](https://dspy.ai), [PromptFlow](https://microsoft.github.io/promptflow/) — open-sourced here |

---

## Star History

[![Star History Chart](https://api.star-history.com/svg?repos=hmzainjamil/agentic-patterns-library&type=Date)](https://star-history.com/#hmzainjamil/agentic-patterns-library&Date)

---

<div align="center">
Built by <a href="https://github.com/hmzainjamil">HMZ</a> · Production agent patterns from DigiMinds ops
</div>
