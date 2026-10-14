# Automation — `automation` skills

Repeatable pipelines: recon automation, nuclei templates, browser-driven testing, and continuous monitoring.

## Skills in this domain

- [`automation-browser`](automation-browser/SKILL.md) — Drive a real browser against an in-scope web app with Playwright / agent-browser: automated login, form and payload submission through the UI, scraping JS-rendered pages, request/response interception, and evidence screenshots.
- [`automation-nuclei-templates`](automation-nuclei-templates/SKILL.md) — Write custom nuclei templates to codify a finding into a repeatable, mass-scannable check.
- [`automation-recon-pipeline`](automation-recon-pipeline/SKILL.md) — Chain recon tools into a repeatable, resumable pipeline for continuous bug-bounty coverage.

Add a skill here:
```bash
cp -r skills/_templates/technique.md skills/automation/<slug>/SKILL.md
# edit frontmatter (domain: automation) + body, then:
python3 tools/catalog.py
```

Naming: domain-prefixed kebab-case, e.g. `automation-<thing>`. See the full table in [`CATALOG.md`](../../docs/CATALOG.md).
