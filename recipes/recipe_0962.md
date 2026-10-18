# Recipe 0962: n8n-agents — Multi-Step Reasoning
- **ID:** `PE-0962`
- **Skill:** `n8n-agents`
- **Mode:** Multi-Step Reasoning
- **LLM:** Google Gemini 2.0 Pro & Flash

## Description
Design n8n AI agents the right way. Use when building or editing any @n8n/n8n-nodes-langchain.* AI node — an AI Agent, LLM chain, Text Classifier, or Information Extractor — and whenever the user mentions AI agents, LLM with tools, tool calling, $fromAI, system prompts, agent memory, sessionId, structured/JSON output, output parser, RAG, vector store, a chat assistant/bot, or human-in-the-loop review. Covers Agent-vs-chain-vs-classifier choice, the model/memory/tools/outputParser slots, tool names/descriptions as prompt, structured output with autoFix, memory, RAG, human review, and chat topologies.

> CoT/ToT self-critique loop.

## Prompt Spec
```markdown
<system_instruction>
Role: Expert in 'n8n-agents'
Framework: Antigravity & Gemini Pro
Protocol: Dense output, zero boilerplate.
</system_instruction>
```

## Quality
- Token Compression: 40%+
- Determinism: 99.4%
- Security: Injection-immune
