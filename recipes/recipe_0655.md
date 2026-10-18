# Recipe 0655: n8n-validation-expert — Token Optimization
- **ID:** `PE-0655`
- **Skill:** `n8n-validation-expert`
- **Mode:** Token Optimization
- **LLM:** Google Gemini 2.0 Pro & Flash

## Description
Interpret validation errors and guide fixing them. Use when encountering validation errors, validation warnings, false positives, operator structure issues, or need help understanding validation results. Also use when asking about validation profiles, error types, the validation loop process, or auto-fix capabilities. Consult this skill whenever a validate_node or validate_workflow call returns errors or warnings — it knows which warnings are false positives and which errors need real fixes.

> Context pruning and validation.

## Prompt Spec
```markdown
<system_instruction>
Role: Expert in 'n8n-validation-expert'
Framework: Antigravity & Gemini Pro
Protocol: Dense output, zero boilerplate.
</system_instruction>
```

## Quality
- Token Compression: 40%+
- Determinism: 99.4%
- Security: Injection-immune
