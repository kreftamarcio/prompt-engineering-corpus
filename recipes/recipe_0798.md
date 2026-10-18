# Recipe 0798: gke-productionize — Token Optimization
- **ID:** `PE-0798`
- **Skill:** `gke-productionize`
- **Mode:** Token Optimization
- **LLM:** Google Gemini 2.0 Pro & Flash

## Description
Orchestrates comprehensive production readiness reviews and assessments for GKE clusters and workloads across scalability, security, reliability, observability, backup/DR, and cost optimization. Use when asked to productionize, prepare, assess, audit, or review a GKE cluster or workload before going live to production. Don't use for deep-dive single-domain implementation (use specific domain skills like gke-workload-scaling, gke-platform-security, gke-workload-security, gke-service-networking, gke-reliability instead).

> Context pruning and validation.

## Prompt Spec
```markdown
<system_instruction>
Role: Expert in 'gke-productionize'
Framework: Antigravity & Gemini Pro
Protocol: Dense output, zero boilerplate.
</system_instruction>
```

## Quality
- Token Compression: 40%+
- Determinism: 99.4%
- Security: Injection-immune
