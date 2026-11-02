# Prompt Engineering Corpus

[![Python](https://img.shields.io/badge/Python-3.12+-3776AB?logo=python&logoColor=white)](https://python.org)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

Personal collection of **prompt and context engineering patterns** for LLMs and AI agents, written in Markdown, plus a small Python CLI that builds a structured "context contract" from a goal.

Maintained by [Márcio Krefta](https://github.com/kreftamarcio) ([Q1 by TACO](https://github.com/q1-by-taco)).

## Contents

```
prompt-engineering-corpus/
├── docs/
│   ├── CONTEXT_ENGINEERING_MANIFESTO.md        # notes on context engineering
│   └── THE_8_PILLARS_OF_CONTEXT_ENGINEERING.md # the 8 principles used to organize the recipes
├── tools/
│   └── context_compiler.py                     # CLI that generates a context contract
├── recipes/                                    # prompt / context recipes in Markdown
└── README.md
```

## The 8 principles

| # | Principle | Idea |
|---|---|---|
| 01 | Prefix-stable prompts | Keep the fixed part of the prompt at the top and unchanged, so providers that support prompt caching can reuse it. |
| 02 | Delimiters for untrusted content | Wrap external content in explicit tags (e.g. `<untrusted_payload>`) to reduce indirect prompt injection. |
| 03 | Evidence-first | Ask the agent to verify with tests or execution output before declaring a task done. |
| 04 | MCP for tools | Expose tools through the Model Context Protocol instead of ad-hoc integrations. |
| 05 | Working-memory management | Drop stale tool outputs and keep the context window within a budget. |
| 06 | Context pruning | Remove redundant text before sending it to the model. |
| 07 | Structured outputs | Use JSON schemas / typed models to constrain responses. |
| 08 | Continuous evaluation | Keep regression prompts and run them when prompts change. |

## Usage

```bash
git clone https://github.com/kreftamarcio/prompt-engineering-corpus.git
cd prompt-engineering-corpus

python3 tools/context_compiler.py \
  --name "autonomous-agent-optimizer" \
  --domain "AI Engineering" \
  --objective "Audit pull requests, run test verification and enforce conventional commits"
```

> **Note:** these recipes are reference patterns and have not been benchmarked against production models in this repository.
