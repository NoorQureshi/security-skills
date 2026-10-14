# Privilege escalation — `privesc` skills

Local privilege escalation on Linux and Windows: misconfig quick-wins first, then deeper vectors toward root/SYSTEM.

## Skills in this domain

- [`privesc-arsenal`](privesc-arsenal/SKILL.md) — Linux + Windows local privilege-escalation tool arsenal for authorized engagements.
- [`privesc-enumeration`](privesc-enumeration/SKILL.md) — Systematic post-foothold host enumeration and credential/loot hunting on Linux and Windows — build situational awareness and find the lead that escalates or moves laterally.
- [`privesc-linux-gtfobins`](privesc-linux-gtfobins/SKILL.md) — Linux privilege escalation via sudo rules, SUID/SGID binaries, and capabilities using GTFOBins techniques.
- [`privesc-windows-tokens`](privesc-windows-tokens/SKILL.md) — Windows privilege escalation via token impersonation privileges — SeImpersonate/SeAssignPrimaryToken (the Potato family) and related token abuse to SYSTEM.

Add a skill here:
```bash
cp -r skills/_templates/technique.md skills/privesc/<slug>/SKILL.md
# edit frontmatter (domain: privesc) + body, then:
python3 tools/catalog.py
```

Naming: domain-prefixed kebab-case, e.g. `privesc-<thing>`. See the full table in [`CATALOG.md`](../../docs/CATALOG.md).
