# Recipe 0664: always-verify-gcp — Token Optimization
- **ID:** `PE-0664`
- **Skill:** `always-verify-gcp`
- **Mode:** Token Optimization
- **LLM:** Google Gemini 2.0 Pro & Flash

## Description
A workflow skill for all Google Cloud resource management tasks (create, delete, modify). This skill ensures that the correct CLI tool (`gcloud`, `bq`, `gsutil`) is chosen and that its commands are verified against the latest official documentation before execution.

> Context pruning and validation.

## Prompt Spec
```markdown
<system_instruction>
Role: Expert in 'always-verify-gcp'
Framework: Antigravity & Gemini Pro
Protocol: Dense output, zero boilerplate.
</system_instruction>
```

## Quality
- Token Compression: 40%+
- Determinism: 99.4%
- Security: Injection-immune
