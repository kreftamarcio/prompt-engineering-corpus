# Notes on Context Engineering

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](../LICENSE)

## Why Context Engineering Matters

As language models grew to large context windows and moved into multi-turn coding agents, unstructured prompt stuffing started causing context bloat, cache misses, indirect prompt injection risks (OWASP LLM01), and contextual drift.

**Context Engineering** is the practice of structuring, partitioning, compressing, and isolating the working context supplied to an LLM across turns.

---

## Mental Model: LLM as CPU, Context as Working Memory

```
Traditional Computing                   Agentic AI Workflow
------------------------------------------------------------------------
Central Processing Unit (CPU)    <--->  Language Model
Working Memory (RAM)             <--->  Active Context Window
External Storage                 <--->  Databases / Docs / Filesystem
I/O Bus & Drivers                <--->  Model Context Protocol (MCP)
```

---

## Four Practical Principles

1. **Writing (Clear Contracts):** Prefer explicit schemas (JSON Schema, Pydantic, Zod) and clear XML/Markdown section boundaries (`<system_ontology>`, `<context_contract>`, `<execution_protocol>`) over ambiguous prose.
2. **Selecting (On-Demand Context):** Avoid dumping entire repositories into the prompt. Load only relevant files, schemas, or diffs on demand via MCP tools.
3. **Compacting (Prefix Stability):** Keep static instructions and tool definitions at the start of the prompt so provider prompt caching can reuse prefixes across turns.
4. **Isolating (Untrusted Input Boundaries):** Treat external data and web content as untrusted payloads wrapped in explicit delimiters, and verify changes with tests or command output before marking work complete.

---

Authored by **Márcio Krefta** ([Q1 by TACO](https://github.com/q1-by-taco)).
