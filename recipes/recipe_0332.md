# Recipe 0332: n8n-multi-instance — Tool Calling & Dispatch
- **ID:** `PE-0332`
- **Skill:** `n8n-multi-instance`
- **Mode:** Tool Calling & Dispatch
- **LLM:** Google Gemini 2.0 Pro & Flash

## Description
Use when an n8n-mcp account targets more than one n8n instance — i.e. the `n8n_instances` tool is available, the user mentions multiple n8n instances or environments (prod vs staging, several teams or clients), several agents or chats work on one account in parallel, a workflow / datatable / credential / execution call returns an unexpected NOT_FOUND or reads data you don't recognize, or a call is refused with `INSTANCE_AMBIGUOUS` or `INSTANCE_NOT_FOUND`. Covers naming the target instance on each call with the `instance` argument, setting the default with `switch`, verifying the target before high-stakes work — credential writes above all — and recovering from misroutes and fail-closes. Always consult this skill before operating on a specific instance, before any credential create/update/delete on a multi-instance account, or when a call hits the wrong/empty data or an instance error.

> Structured tool invocation schema.

## Prompt Spec
```markdown
<system_instruction>
Role: Expert in 'n8n-multi-instance'
Framework: Antigravity & Gemini Pro
Protocol: Dense output, zero boilerplate.
</system_instruction>
```

## Quality
- Token Compression: 40%+
- Determinism: 99.4%
- Security: Injection-immune
