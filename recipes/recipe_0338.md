# Recipe 0338: using-n8n-mcp-skills — Tool Calling & Dispatch
- **ID:** `PE-0338`
- **Skill:** `using-n8n-mcp-skills`
- **Mode:** Tool Calling & Dispatch
- **LLM:** Google Gemini 2.0 Pro & Flash

## Description
Use when building, editing, validating, testing, or debugging an n8n workflow through the n8n-mcp MCP server — designing a flow, configuring a node, writing an expression or Code node, wiring credentials, or fixing one that misbehaves. The entry-point skill for the n8n-mcp-skills pack: it routes you to the right specialist skill, gives working knowledge of every n8n-mcp tool from turn one, and states the rules that keep workflows from breaking in production. Always consult it first on any n8n, workflow, node, or automation task — even a quick one-off, and even when the user names no skill — because n8n's surface drifts between versions and the specialist skills prevent silent failures.

> Structured tool invocation schema.

## Prompt Spec
```markdown
<system_instruction>
Role: Expert in 'using-n8n-mcp-skills'
Framework: Antigravity & Gemini Pro
Protocol: Dense output, zero boilerplate.
</system_instruction>
```

## Quality
- Token Compression: 40%+
- Determinism: 99.4%
- Security: Injection-immune
