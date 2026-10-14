# Tradecraft & discipline — `tradecraft` skills

How to operate: the dual-mode scope/RoE rule, complex multi-stage engagement discipline, rabbit-hole tracking, and multi-host method.

## Skills in this domain

- [`tradecraft-attack-chain`](tradecraft-attack-chain/SKILL.md) — Orchestrate a full multi-stage kill chain — recon → initial access → privilege escalation → lateral movement → objective — with phase gates, per-phase playbooks, and operating discipline.
- [`tradecraft-attack-path-mapping`](tradecraft-attack-path-mapping/SKILL.md) — Model the target as an attack graph — nodes (assets, identities, trust) and edges (a technique that gets you from one to the next) — and find the shortest path to the objective.
- [`tradecraft-attack-scenarios`](tradecraft-attack-scenarios/SKILL.md) — Turn a goal + a scope into a concrete, ordered attack scenario across multiple skills — not one technique in isolation.
- [`tradecraft-bugbounty-platforms`](tradecraft-bugbounty-platforms/SKILL.md) — Understand how the major bug-bounty platforms differ — scope rules, disclosure, triage, and reputation — so you play each correctly.
- [`tradecraft-complex-engagements`](tradecraft-complex-engagements/SKILL.md) — Structure and discipline for complex, multi-stage targets — where the path is a chain of several bugs across multiple hosts, needs source review / custom exploit work, and spans sessions.
- [`tradecraft-duplicate-avoidance`](tradecraft-duplicate-avoidance/SKILL.md) — Avoid burning time on bugs that will be closed as duplicates.
- [`tradecraft-pivot-decisions`](tradecraft-pivot-decisions/SKILL.md) — Decide what to do next after a result — the branching logic that turns a single outcome into the next lead.
- [`tradecraft-scope-roe`](tradecraft-scope-roe/SKILL.md) — Establish and enforce the authorization envelope before any testing — the scope rule that governs everything.
- [`tradecraft-target-selection`](tradecraft-target-selection/SKILL.md) — Choose where to spend effort for the best return — which program, which asset, which surface.

Add a skill here:
```bash
cp -r skills/_templates/technique.md skills/tradecraft/<slug>/SKILL.md
# edit frontmatter (domain: tradecraft) + body, then:
python3 tools/catalog.py
```

Naming: domain-prefixed kebab-case, e.g. `tradecraft-<thing>`. See the full table in [`CATALOG.md`](../../docs/CATALOG.md).
