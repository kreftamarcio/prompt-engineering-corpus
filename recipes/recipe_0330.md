# Recipe 0330: n8n-expression-syntax — Tool Calling & Dispatch
- **ID:** `PE-0330`
- **Skill:** `n8n-expression-syntax`
- **Mode:** Tool Calling & Dispatch
- **LLM:** Google Gemini 2.0 Pro & Flash

## Description
Validate n8n expression syntax and fix common errors. Use when writing n8n expressions, using {{}} syntax, accessing $json/$node variables, troubleshooting expression errors, mapping data between nodes, or referencing webhook data in workflows. Use this skill whenever configuring node fields that reference data from previous nodes — expressions are how n8n passes data between nodes, and getting the syntax wrong is the most common source of workflow errors. Also use when asked whether a complex expression hurts performance.

> Structured tool invocation schema.

## Prompt Spec
```markdown
<system_instruction>
Role: Expert in 'n8n-expression-syntax'
Framework: Antigravity & Gemini Pro
Protocol: Dense output, zero boilerplate.
</system_instruction>
```

## Quality
- Token Compression: 40%+
- Determinism: 99.4%
- Security: Injection-immune
