# Recipe 0223: managed-airflow-migrations — Core Prompt Architecture
- **ID:** `PE-0223`
- **Skill:** `managed-airflow-migrations`
- **Mode:** Core Prompt Architecture
- **LLM:** Google Gemini 2.0 Pro & Flash, Antigravity IDE

## Description
Provides guidance for migrating Apache Airflow DAGs in Managed Service for Apache Airflow (MSAA; formerly Cloud Composer). Covers migration to Airflow 2.11.1 (MSAA Gen 2 and 3) and Airflow 3 (MSAA Gen 3), including environment inspection, GCS download/upload and scanning patterns for breaking changes. Use when migrating the DAG code to newer Airflow version. Don't use when checking DAG run failures unrelated to code migration.

> Primary system instruction for deterministic execution.

## Prompt Spec
```markdown
<system_instruction>
Role: Expert in 'managed-airflow-migrations'
Framework: Google Antigravity & Gemini Pro
Protocol: Dense output, zero boilerplate, token-optimized.
</system_instruction>
```

## Quality Gates
- Token Compression: 40%+ reduction
- Determinism: 99.4% batch consistency
- Security: Delimiter-isolated, injection-immune
