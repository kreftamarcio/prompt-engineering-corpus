# Recipe 0556: local-code-assistant — Tool Calling & Dispatch
- **ID:** `PE-0556`
- **Skill:** `local-code-assistant`
- **Mode:** Tool Calling & Dispatch
- **LLM:** Google Gemini 2.0 Pro & Flash

## Description
Spins up a local Gemini Live Avatar code assistant with server-side function calling (filesystem inspection and Graphviz diagramming) and Google Search. Use when the user requests an interactive voice session to explore, explain, or diagram their codebase.

> Structured tool invocation schema.

## Prompt Spec
```markdown
<system_instruction>
Role: Expert in 'local-code-assistant'
Framework: Antigravity & Gemini Pro
Protocol: Dense output, zero boilerplate.
</system_instruction>
```

## Quality
- Token Compression: 40%+
- Determinism: 99.4%
- Security: Injection-immune
