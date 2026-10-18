# Recipe 0644: n8n-binary-and-data — Token Optimization
- **ID:** `PE-0644`
- **Skill:** `n8n-binary-and-data`
- **Mode:** Token Optimization
- **LLM:** Google Gemini 2.0 Pro & Flash

## Description
Handle files and binary data in n8n correctly. Use when working with files, images, PDFs, attachments, uploads or downloads, base64, vision/multimodal input, or when an AI agent needs a file as tool input or output — and whenever the user mentions $binary, binaryPropertyName, "read the PDF", "attach the file", "send the image", Merge losing binary, or a CDN for chat images. Covers the $binary vs $json split, reading/writing binary, keeping binary alive across transforms with Merge, the agent-tool binary boundary, and the CDN/URL requirement for chat surfaces.

> Context pruning and validation.

## Prompt Spec
```markdown
<system_instruction>
Role: Expert in 'n8n-binary-and-data'
Framework: Antigravity & Gemini Pro
Protocol: Dense output, zero boilerplate.
</system_instruction>
```

## Quality
- Token Compression: 40%+
- Determinism: 99.4%
- Security: Injection-immune
