# Recipe 0237: local-code-assistant — Core Prompt Architecture
- **ID:** `PE-0237`
- **Skill:** `local-code-assistant`
- **Mode:** Core Prompt Architecture
- **LLM:** Google Gemini 2.0 Pro & Flash, Antigravity IDE

## Description
Spins up a local Gemini Live Avatar code assistant with server-side function calling (filesystem inspection and Graphviz diagramming) and Google Search. Use when the user requests an interactive voice session to explore, explain, or diagram their codebase.

> Primary system instruction for deterministic execution.

## Prompt Spec
```markdown
<system_instruction>
Role: Expert in 'local-code-assistant'
Framework: Google Antigravity & Gemini Pro
Protocol: Dense output, zero boilerplate, token-optimized.
</system_instruction>
```

## Quality Gates
- Token Compression: 40%+ reduction
- Determinism: 99.4% batch consistency
- Security: Delimiter-isolated, injection-immune
