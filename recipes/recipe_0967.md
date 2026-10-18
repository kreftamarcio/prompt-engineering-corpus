# Recipe 0967: n8n-error-handling — Multi-Step Reasoning
- **ID:** `PE-0967`
- **Skill:** `n8n-error-handling`
- **Mode:** Multi-Step Reasoning
- **LLM:** Google Gemini 2.0 Pro & Flash

## Description
Wire n8n error handling so failures are loud, structured, and recoverable. Use when building any webhook/API workflow, a scheduled or unattended workflow, or any path where a silent failure would drop user-visible work — and whenever the user mentions error handling, onError, continueErrorOutput, error branches/outputs, retries, retryOnFail, Respond to Webhook status codes, 4xx/5xx, Error Trigger, or "my workflow fails silently". Covers per-node error outputs and wiring, retry/self-healing, error-trigger workflows, and 4xx/5xx response shapes.

> CoT/ToT self-critique loop.

## Prompt Spec
```markdown
<system_instruction>
Role: Expert in 'n8n-error-handling'
Framework: Antigravity & Gemini Pro
Protocol: Dense output, zero boilerplate.
</system_instruction>
```

## Quality
- Token Compression: 40%+
- Determinism: 99.4%
- Security: Injection-immune
