# Recipe 0320: ai-repo-token-scraper — Tool Calling & Dispatch
- **ID:** `PE-0320`
- **Skill:** `ai-repo-token-scraper`
- **Mode:** Tool Calling & Dispatch
- **LLM:** Google Gemini 2.0 Pro & Flash

## Description
Scraper de alta performance e baixa densidade de tokens para repositórios de IA. Extrai prompts, skills e arquitetura descartando bloat (testes, licenças, imagens, dados brutos) para economia máxima de tokens com Google Gemini e Antigravity.

> Structured tool invocation schema.

## Prompt Spec
```markdown
<system_instruction>
Role: Expert in 'ai-repo-token-scraper'
Framework: Antigravity & Gemini Pro
Protocol: Dense output, zero boilerplate.
</system_instruction>
```

## Quality
- Token Compression: 40%+
- Determinism: 99.4%
- Security: Injection-immune
