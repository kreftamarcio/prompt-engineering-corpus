# The 8 Principles of Context Engineering

Practical guidelines used to organize the prompt and context patterns in this repository.

---

## Overview

| # | Principle | Mechanism | Goal |
|---|---|---|---|
| **01. Prefix-Stable Prompts** | Keep static instructions at the top of the prompt | Better provider prompt-cache reuse |
| **02. Delimiter Isolation** | Wrap external content in explicit XML tags | Reduce indirect prompt injection risk (OWASP LLM01) |
| **03. Evidence-First Gates** | Require test or command output before completion | Reduce unverified claims |
| **04. Standardized MCP Tools** | JSON-RPC 2.0 tool interfaces via MCP | Decouple prompts from custom glue code |
| **05. Working Memory Management** | Trim stale tool outputs across long sessions | Keep context within budget |
| **06. Context Pruning** | Remove boilerplate and repetitive text | Lower token usage |
| **07. Structured Outputs** | Validate responses with JSON Schema / Pydantic / Zod | Reliable parsing in application code |
| **08. Regression Checks** | Keep a small set of test prompts when editing templates | Catch regressions early |

---

## Details

### 01. Prefix-Stable Prompts
Keep system instructions and tool schemas stable at the beginning of the prompt and append dynamic turn data at the end so providers that support prefix caching can reuse earlier tokens.

### 02. Delimiter Isolation
Wrap untrusted text (user input, web pages, external documents) in explicit tags such as `<untrusted_payload>` and instruct the model to treat content inside those tags as data rather than instructions.

### 03. Evidence-First Verification
When used in coding or automation workflows, require concrete verification (such as `pytest`, `tsc`, or command exit codes) before declaring a task finished.

### 04. Model Context Protocol (MCP)
Expose local and remote tools over standard JSON-RPC 2.0 schemas so the same server can be connected to different IDEs and agent clients.

### 05. Working Memory Management
In multi-turn sessions, summarize or drop old tool outputs instead of keeping every intermediate result in full detail.

### 06. Context Pruning
Strip redundant filler from prompts and retrieved documents before sending them to the model.

### 07. Structured Outputs
Use typed schemas (Pydantic, Zod, JSON Schema) whenever downstream code consumes the model output.

### 08. Continuous Evaluation
Maintain example inputs and expected structure checks to test prompt changes before adopting them.

---

Documented by **Márcio Krefta** • [Q1 by TACO](https://github.com/q1-by-taco)
