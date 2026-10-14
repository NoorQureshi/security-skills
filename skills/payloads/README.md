# Payloads — `payloads` skills

Curated payload sets and bypass tables: polyglots, WAF evasion, and wordlist pointers referenced by the technique skills.

## Skills in this domain

- [`payloads-file-transfers`](payloads-file-transfers/SKILL.md) — Move files on/off a target when there's no shared drive — upload tools (linpeas, nc, exploits), pull loot back, and do it through a pivot or when wget/curl are missing.
- [`payloads-reverse-shells`](payloads-reverse-shells/SKILL.md) — Get a reliable reverse (or bind) shell and upgrade it to a real interactive TTY.
- [`payloads-waf-bypass`](payloads-waf-bypass/SKILL.md) — Bypass WAFs/filters blocking your payloads.
- [`payloads-xss-polyglots`](payloads-xss-polyglots/SKILL.md) — Context-breaking XSS polyglots and per-context payloads that fire across HTML/attribute/JS/URL sinks in one shot.

Add a skill here:
```bash
cp -r skills/_templates/technique.md skills/payloads/<slug>/SKILL.md
# edit frontmatter (domain: payloads) + body, then:
python3 tools/catalog.py
```

Naming: domain-prefixed kebab-case, e.g. `payloads-<thing>`. See the full table in [`CATALOG.md`](../../docs/CATALOG.md).
