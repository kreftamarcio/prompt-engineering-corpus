# Recipe 0331: n8n-mcp-tools-expert — Tool Calling & Dispatch
- **ID:** `PE-0331`
- **Skill:** `n8n-mcp-tools-expert`
- **Mode:** Tool Calling & Dispatch
- **LLM:** Google Gemini 2.0 Pro & Flash

## Description
Expert guide for using n8n-mcp MCP tools effectively. Use when searching for nodes, validating configurations, accessing templates, managing workflows, organizing workflows into folders, managing credentials, auditing instance security, or using any n8n-mcp tool. Provides tool selection guidance, parameter formats, and common patterns. IMPORTANT — Always consult this skill before calling any n8n-mcp tool — it prevents common mistakes like wrong nodeType formats, incorrect parameter structures, and inefficient tool usage. If the user mentions n8n, workflows, nodes, or automation and you have n8n MCP tools available, use this skill first.

> Structured tool invocation schema.

## Prompt Spec
```markdown
<system_instruction>
Role: Expert in 'n8n-mcp-tools-expert'
Framework: Antigravity & Gemini Pro
Protocol: Dense output, zero boilerplate.
</system_instruction>
```

## Quality
- Token Compression: 40%+
- Determinism: 99.4%
- Security: Injection-immune
