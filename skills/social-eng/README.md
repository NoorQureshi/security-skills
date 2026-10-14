# Social engineering — `social-eng` skills

Authorized human-factor testing: phishing, vishing/pretexting, and physical assessment — measured
to improve awareness and controls, never to embarrass people. **`pentest`-only, and stricter on
authorization than any other domain.**

> Load [`social-eng-methodology`](social-eng-methodology/SKILL.md) **first**. Social engineering
> tests real people, so it requires written sign-off from someone empowered to consent for the
> staff being tested, agreed pretext/target boundaries, a no-harm line, and a carried authorization
> letter for physical work. No consent → do not run it.

## Skills in this domain

- [`social-eng-methodology`](social-eng-methodology/SKILL.md) — Plan and run an AUTHORIZED social-engineering assessment safely — the load-first guardrails for any human-factor test.
- [`social-eng-phishing`](social-eng-phishing/SKILL.md) — Run an authorized phishing / spear-phishing assessment that measures human-factor risk — pretext, delivery, landing page, and tracking — without harming staff or hoarding real data.
- [`social-eng-physical`](social-eng-physical/SKILL.md) — Run an authorized physical social-engineering assessment — tailgating, pretext entry, badge/RFID cloning checks, and media-drop tests — to measure physical and human access controls safely.
- [`social-eng-vishing-pretext`](social-eng-vishing-pretext/SKILL.md) — Run authorized voice-phishing (vishing) and pretext-based scenarios that test whether staff and help desks follow verification procedures — safely and by consent.

Add a skill here:
```bash
cp -r skills/_templates/methodology.md skills/social-eng/<slug>/SKILL.md
# edit frontmatter (domain: social-eng, modes: [pentest]) + body, then:
python3 tools/catalog.py
```

Naming: domain-prefixed kebab-case, e.g. `social-eng-<thing>`. See the full table in [`CATALOG.md`](../../docs/CATALOG.md).
