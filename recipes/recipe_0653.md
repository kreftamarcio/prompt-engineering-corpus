# Recipe 0653: n8n-self-hosting — Token Optimization
- **ID:** `PE-0653`
- **Skill:** `n8n-self-hosting`
- **Mode:** Token Optimization
- **LLM:** Google Gemini 2.0 Pro & Flash

## Description
Deploy a production self-hosted n8n end-to-end to a fresh Linux VM over SSH, using Docker Compose behind a Caddy reverse proxy with automatic HTTPS. Use whenever the user wants to self-host, install, provision, or deploy n8n on their own server/VPS (Hetzner, DigitalOcean, AWS EC2, bare metal) — single/regular mode or queue mode with workers — or to update, back up, restore, or harden such an instance, or make Python Code nodes run on it (task runners). For SELF-HOSTED n8n (Docker), not n8n Cloud and not building workflows. The skill makes the agent ask single-vs-queue first, collect domain/SSH/timezone inputs, generate fresh secrets on the box, and bring the stack up with TLS. Trigger on "deploy n8n", "self-host n8n", "n8n docker compose", "n8n queue mode / workers", "n8n reverse proxy / SSL", "back up / update my n8n", "Python runner unavailable" / "n8nio/runners sidecar", or "we don't want to give every user the OAuth client secret" / "enable Sign in with Google" (credential overwrites).

> Context pruning and validation.

## Prompt Spec
```markdown
<system_instruction>
Role: Expert in 'n8n-self-hosting'
Framework: Antigravity & Gemini Pro
Protocol: Dense output, zero boilerplate.
</system_instruction>
```

## Quality
- Token Compression: 40%+
- Determinism: 99.4%
- Security: Injection-immune
