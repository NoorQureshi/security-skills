# Reconnaissance — `recon` skills

Passive/active enumeration, OSINT, subdomain discovery, tech fingerprinting, content/param discovery — building the attack surface before you touch it.

## Skills in this domain

- [`recon-arsenal`](recon-arsenal/SKILL.md) — Port/host/service discovery tool arsenal for authorized engagements.
- [`recon-cloud-assets`](recon-cloud-assets/SKILL.md) — Discover an organization's cloud footprint — buckets, blobs, apps, IP ranges, and services across AWS/GCP/Azure.
- [`recon-content-discovery`](recon-content-discovery/SKILL.md) — Discover hidden paths, endpoints, params, and JS-exposed routes on a web target.
- [`recon-dns-analysis`](recon-dns-analysis/SKILL.md) — Deep DNS analysis for attack surface — record mining, zone transfers, DNSSEC/NSEC walking, and dangling records.
- [`recon-github-code-leaks`](recon-github-code-leaks/SKILL.md) — Find secrets and internal detail an organisation leaked to public code — GitHub/GitLab repos, gists, and commit history.
- [`recon-js-analysis`](recon-js-analysis/SKILL.md) — Mine JavaScript for endpoints, params, secrets, and hidden functionality.
- [`recon-osint`](recon-osint/SKILL.md) — Passive OSINT to expand attack surface without touching the target: dorks, code/secret leaks, Shodan/Censys, cloud assets, employees.
- [`recon-subdomain-enum`](recon-subdomain-enum/SKILL.md) — Enumerate subdomains and live hosts to build the attack surface for a bug-bounty program or external assessment.
- [`recon-techstack-fingerprinting`](recon-techstack-fingerprinting/SKILL.md) — Passively identify a target's full technology stack — frontend framework, backend runtime, server, CMS, CDN/WAF, cloud, and versions — from public signals, then route to the right attack skills and CVEs.

Add a skill here:
```bash
cp -r skills/_templates/technique.md skills/recon/<slug>/SKILL.md
# edit frontmatter (domain: recon) + body, then:
python3 tools/catalog.py
```

Naming: domain-prefixed kebab-case, e.g. `recon-<thing>`. See the full table in [`CATALOG.md`](../../docs/CATALOG.md).
