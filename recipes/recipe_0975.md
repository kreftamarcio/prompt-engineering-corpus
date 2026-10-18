# Recipe 0975: n8n-workflow-patterns — Multi-Step Reasoning
- **ID:** `PE-0975`
- **Skill:** `n8n-workflow-patterns`
- **Mode:** Multi-Step Reasoning
- **LLM:** Google Gemini 2.0 Pro & Flash

## Description
Proven workflow architectural patterns from real n8n workflows. Use when building new workflows, designing workflow structure, choosing workflow patterns, planning workflow architecture, or asking about webhook processing, HTTP API integration, database operations, AI agent workflows, batch processing, or scheduled tasks. Always consult this skill when the user asks to create, build, or design an n8n workflow, automate a process, or connect services — even if they don't explicitly mention 'patterns'. Covers webhook, API, database, AI, batch processing, and scheduled automation architectures. Also use when optimizing a slow workflow or speeding up large-item-count processing (node count, batchSize, all-items vs per-item).

> CoT/ToT self-critique loop.

## Prompt Spec
```markdown
<system_instruction>
Role: Expert in 'n8n-workflow-patterns'
Framework: Antigravity & Gemini Pro
Protocol: Dense output, zero boilerplate.
</system_instruction>
```

## Quality
- Token Compression: 40%+
- Determinism: 99.4%
- Security: Injection-immune
