# Reporting — `reporting` skills

Turning findings into deliverables: bug-bounty reports, CVSS/VRT severity, disclosure hygiene, and pentest write-ups.

## Skills in this domain

- [`reporting-bug-bounty-writeup`](reporting-bug-bounty-writeup/SKILL.md) — Turn a confirmed finding into a triage-friendly bug-bounty report (HackerOne/Bugcrowd) with correct severity and clean evidence.
- [`reporting-cvss-scoring`](reporting-cvss-scoring/SKILL.md) — Assign a defensible severity to a finding — build the CVSS 3.1 vector from demonstrated impact and reconcile it with the program's own scale.
- [`reporting-evidence-review`](reporting-evidence-review/SKILL.md) — Pre-handoff audit of an engagement package — scope confirmed, every finding traceable to reproducible evidence, activity-log leads closed with rationale, artifact hashes intact.
- [`reporting-pentest-report`](reporting-pentest-report/SKILL.md) — Structure a professional penetration-test report (engagement deliverable, not a single bug).
- [`reporting-triage-communication`](reporting-triage-communication/SKILL.md) — Work productively with triagers after you submit — answer follow-ups, and handle duplicate, not-applicable, or severity disputes professionally.
- [`reporting-triage-validation`](reporting-triage-validation/SKILL.md) — Validate a finding BEFORE you write it up — kill false positives, confirm real impact, check scope, and deduplicate.

Add a skill here:
```bash
cp -r skills/_templates/technique.md skills/reporting/<slug>/SKILL.md
# edit frontmatter (domain: reporting) + body, then:
python3 tools/catalog.py
```

Naming: domain-prefixed kebab-case, e.g. `reporting-<thing>`. See the full table in [`CATALOG.md`](../../docs/CATALOG.md).
