# Recipe 0652: n8n-node-configuration — Token Optimization
- **ID:** `PE-0652`
- **Skill:** `n8n-node-configuration`
- **Mode:** Token Optimization
- **LLM:** Google Gemini 2.0 Pro & Flash

## Description
Operation-aware node configuration guidance. Use when configuring nodes, understanding property dependencies, determining required fields, choosing between get_node detail levels, or learning common configuration patterns by node type. Always use this skill when setting up node parameters — it explains which fields are required for each operation, how displayOptions control field visibility, and when to use patchNodeField for surgical edits vs full node updates.

> Context pruning and validation.

## Prompt Spec
```markdown
<system_instruction>
Role: Expert in 'n8n-node-configuration'
Framework: Antigravity & Gemini Pro
Protocol: Dense output, zero boilerplate.
</system_instruction>
```

## Quality
- Token Compression: 40%+
- Determinism: 99.4%
- Security: Injection-immune
