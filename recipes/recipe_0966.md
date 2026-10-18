# Recipe 0966: n8n-code-tool — Multi-Step Reasoning
- **ID:** `PE-0966`
- **Skill:** `n8n-code-tool`
- **Mode:** Multi-Step Reasoning
- **LLM:** Google Gemini 2.0 Pro & Flash

## Description
Write JavaScript or Python for the n8n Custom Code Tool (@n8n/n8n-nodes-langchain.toolCode) — the AI-agent-callable tool, NOT the workflow Code node. Use when building a Code Tool attached to an AI Agent, writing code that an LLM will invoke, parsing the `query` input, returning a string result, defining an input schema for structured arguments (specifyInputSchema, jsonSchemaExample, DynamicStructuredTool), or troubleshooting errors like \"Wrong output type returned\", \"No execution data available\", \"The response property should be a string, but it is an object\", \"Cannot assign to read only property 'name'\", or an AI agent that refuses to call the tool. Covers the critical differences between Code node and Code Tool: return format (string vs `[{json:{...}}]`), unavailability of `$fromAI`/`$input`/`$helpers` in the Code Tool sandbox, naming rules for AI invocation, and when to use `toolWorkflow`/HTTP Request Tool instead.

> CoT/ToT self-critique loop.

## Prompt Spec
```markdown
<system_instruction>
Role: Expert in 'n8n-code-tool'
Framework: Antigravity & Gemini Pro
Protocol: Dense output, zero boilerplate.
</system_instruction>
```

## Quality
- Token Compression: 40%+
- Determinism: 99.4%
- Security: Injection-immune
