# AI / LLM — `ai-ml` skills

Attacks on LLM-backed apps and agents: prompt injection (direct/indirect), data exfil, tool/function abuse, jailbreaks — OWASP LLM Top 10.

## Skills in this domain

- [`ai-agent-tool-abuse`](ai-agent-tool-abuse/SKILL.md) — Abuse an LLM agent's tools/functions — coerce it to call tools with attacker-chosen args for SSRF, RCE, data exfil, or privilege abuse.
- [`ai-insecure-output-handling`](ai-insecure-output-handling/SKILL.md) — Exploit apps that trust LLM output — pass model text unsanitized into XSS sinks, SQL, shell, code, or downstream calls.
- [`ai-jailbreak`](ai-jailbreak/SKILL.md) — Bypass an LLM's safety/guardrails to make it produce restricted output or ignore its policy.
- [`ai-llm-dos`](ai-llm-dos/SKILL.md) — Unbounded-consumption / denial-of-wallet attacks on LLM apps — force runaway tokens, cost, or latency.
- [`ai-mcp-security`](ai-mcp-security/SKILL.md) — Assess Model Context Protocol (MCP) servers and agent tool integrations — tool poisoning, prompt injection via tool descriptions/results, over-broad scopes, and unauth tool exposure.
- [`ai-model-extraction`](ai-model-extraction/SKILL.md) — Extract or steal an ML/LLM model's parameters, training data, or system prompt via query access — model stealing, membership inference, training-data extraction.
- [`ai-prompt-injection`](ai-prompt-injection/SKILL.md) — Test LLM-backed apps for prompt injection (direct + indirect) and its consequences: data exfil, tool/function abuse, guardrail bypass.
- [`ai-rag-poisoning`](ai-rag-poisoning/SKILL.md) — Poison a RAG/knowledge-base pipeline so retrieved content hijacks the model (indirect prompt injection at scale) or exfiltrates data.
- [`ai-sensitive-data-disclosure`](ai-sensitive-data-disclosure/SKILL.md) — Make an LLM app disclose sensitive data it should never reveal: training-data memorization, secrets/PII in RAG context, cross-tenant leakage, conversation logs.
- [`ai-supply-chain`](ai-supply-chain/SKILL.md) — Attack the ML/LLM supply chain — poisoned models, datasets, plugins, and unsafe model deserialization.
- [`ai-system-prompt-leakage`](ai-system-prompt-leakage/SKILL.md) — Extract an LLM app's system prompt / hidden developer instructions — the attack map that reveals guardrails, tool definitions, internal endpoints, and planted secrets.

Add a skill here:
```bash
cp -r skills/_templates/technique.md skills/ai-ml/<slug>/SKILL.md
# edit frontmatter (domain: ai-ml) + body, then:
python3 tools/catalog.py
```

Naming: domain-prefixed kebab-case, e.g. `ai-ml-<thing>`. See the full table in [`CATALOG.md`](../../docs/CATALOG.md).
