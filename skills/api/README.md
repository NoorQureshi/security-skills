# API — `api` skills

REST/GraphQL/gRPC attacks: BOLA/BFLA, mass assignment, injection, introspection abuse — the OWASP API Top 10 surface.

## Skills in this domain

- [`api-auth-attacks`](api-auth-attacks/SKILL.md) — Break API authentication: token handling, key leakage, weak session/JWT, and no-auth endpoints.
- [`api-bola`](api-bola/SKILL.md) — Broken Object/Function Level Authorization in REST/JSON APIs (the #1 API risk).
- [`api-fuzzing`](api-fuzzing/SKILL.md) — Discover and fuzz API endpoints, methods, params, and versions systematically.
- [`api-graphql`](api-graphql/SKILL.md) — Attack GraphQL APIs.
- [`api-grpc`](api-grpc/SKILL.md) — Test gRPC / Protocol Buffers APIs — reflection, method enumeration, authz, and injection.
- [`api-mass-assignment`](api-mass-assignment/SKILL.md) — Mass assignment / auto-binding privilege escalation.
- [`api-mongo-agg-facet-bypass`](api-mongo-agg-facet-bypass/SKILL.md) — Bypass a MongoDB aggregation-pipeline stage allowlist by nesting disallowed read stages inside `$facet`, then `$unionWith`/`$lookup` sibling collections to exfiltrate secrets.
- [`api-testing-checklist`](api-testing-checklist/SKILL.md) — A fast, ordered methodology for assessing an API end to end — REST/GraphQL/gRPC/SOAP — so nothing gets skipped.
- [`api-versioning`](api-versioning/SKILL.md) — Find and attack old/shadow API versions that missed a fix — improper inventory management.

Add a skill here:
```bash
cp -r skills/_templates/technique.md skills/api/<slug>/SKILL.md
# edit frontmatter (domain: api) + body, then:
python3 tools/catalog.py
```

Naming: domain-prefixed kebab-case, e.g. `api-<thing>`. See the full table in [`CATALOG.md`](../../docs/CATALOG.md).
