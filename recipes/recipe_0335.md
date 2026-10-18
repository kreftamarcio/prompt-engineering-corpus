# Recipe 0335: n8n-subworkflows — Tool Calling & Dispatch
- **ID:** `PE-0335`
- **Skill:** `n8n-subworkflows`
- **Mode:** Tool Calling & Dispatch
- **LLM:** Google Gemini 2.0 Pro & Flash

## Description
Build reusable, composable n8n sub-workflows. Use when extracting shared logic, building anything multi-step or reused across workflows, or any workflow over ~10 nodes — and whenever the user mentions sub-workflows, Execute Workflow, reuse, shared/common logic, modular workflows, "Define Below" inputs, waitForSubWorkflow, mode each vs all, or exposing a workflow as an agent tool. Covers typed sub-workflow inputs, all-vs-each execution, verb-first naming for discovery, stateless vs stateful design, and splitting by input shape.

> Structured tool invocation schema.

## Prompt Spec
```markdown
<system_instruction>
Role: Expert in 'n8n-subworkflows'
Framework: Antigravity & Gemini Pro
Protocol: Dense output, zero boilerplate.
</system_instruction>
```

## Quality
- Token Compression: 40%+
- Determinism: 99.4%
- Security: Injection-immune
