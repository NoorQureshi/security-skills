# Source-code review — `code-review` skills

SAST-style manual review: dangerous sinks per language, secret detection, auth/authz flaws, and vulnerable dependency patterns.

## Skills in this domain

- [`code-review-cicd`](code-review-cicd/SKILL.md) — Review CI/CD pipelines for security flaws — poisoned workflows, secret leakage, and injection.
- [`code-review-cpp`](code-review-cpp/SKILL.md) — Security review of C / C++ code — memory-safety and the classic unsafe-API sinks.
- [`code-review-dangerous-sinks`](code-review-dangerous-sinks/SKILL.md) — Grep-ready dangerous function/sink catalog per language for fast code review.
- [`code-review-dotnet`](code-review-dotnet/SKILL.md) — Security review of .NET / C# code — dangerous sinks and ASP.NET pitfalls.
- [`code-review-go`](code-review-go/SKILL.md) — Security review of Go code — dangerous sinks and web-framework pitfalls.
- [`code-review-iac`](code-review-iac/SKILL.md) — Security review of infrastructure-as-code — Terraform, CloudFormation, Ansible, Kubernetes/Helm manifests.
- [`code-review-java`](code-review-java/SKILL.md) — Security review of Java code — dangerous sinks and Spring pitfalls.
- [`code-review-methodology`](code-review-methodology/SKILL.md) — Systematic manual source-code security review — how to find bugs by reading code.
- [`code-review-nodejs`](code-review-nodejs/SKILL.md) — Security review of Node.js / JavaScript code — dangerous sinks and Express/framework pitfalls.
- [`code-review-php`](code-review-php/SKILL.md) — Security review of PHP code — dangerous sinks and framework pitfalls (Laravel/Symfony/WordPress).
- [`code-review-python`](code-review-python/SKILL.md) — Security review of Python code — dangerous sinks and framework-specific pitfalls (Django/Flask/FastAPI).
- [`code-review-ruby`](code-review-ruby/SKILL.md) — Security review of Ruby code — dangerous sinks and Rails pitfalls.
- [`code-review-rust`](code-review-rust/SKILL.md) — Security review of Rust code — where a memory-safe language still has real bugs: `unsafe`, FFI, panics, and the usual injection/logic sinks.
- [`code-review-secrets-detection`](code-review-secrets-detection/SKILL.md) — Find leaked secrets in code, git history, and CI.
- [`code-review-solidity`](code-review-solidity/SKILL.md) — Security review of Solidity / EVM smart contracts — reentrancy, access control, arithmetic, and DeFi economic bugs.

Add a skill here:
```bash
cp -r skills/_templates/technique.md skills/code-review/<slug>/SKILL.md
# edit frontmatter (domain: code-review) + body, then:
python3 tools/catalog.py
```

Naming: domain-prefixed kebab-case, e.g. `code-review-<thing>`. See the full table in [`CATALOG.md`](../../docs/CATALOG.md).
