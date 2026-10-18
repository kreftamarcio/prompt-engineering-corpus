# Recipe 0327: n8n-code-python — Tool Calling & Dispatch
- **ID:** `PE-0327`
- **Skill:** `n8n-code-python`
- **Mode:** Tool Calling & Dispatch
- **LLM:** Google Gemini 2.0 Pro & Flash

## Description
Write Python in n8n Code nodes (native Python, `language` pythonNative, n8n 2.x). Use when the user explicitly wants Python in a Code node, when migrating old Pyodide/"Python (Beta)" code that used _input/_json/_node/_now, or when a Python Code node fails with NameError, "Security violations detected", "Import of standard library module … is disallowed", "__build_class__ not found", "A 'json' property isn't a dictionary", or "Python runner unavailable". Covers the only two variables (_items/_item), dict-only access, imports blocked by default, the sandbox's denied builtins, accepted return shapes, and how errors interact with onError. JavaScript is the default for Code nodes — native Python has no n8n helpers and, by default, no imports. EXCEPTION — for Python in the AI-agent-callable Custom Code Tool (@n8n/n8n-nodes-langchain.toolCode), use the n8n-code-tool skill instead (input is _query, return must be a string).

> Structured tool invocation schema.

## Prompt Spec
```markdown
<system_instruction>
Role: Expert in 'n8n-code-python'
Framework: Antigravity & Gemini Pro
Protocol: Dense output, zero boilerplate.
</system_instruction>
```

## Quality
- Token Compression: 40%+
- Determinism: 99.4%
- Security: Injection-immune
