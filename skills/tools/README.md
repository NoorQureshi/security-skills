# Tool guides — `tools` skills

How to drive the actual offensive tooling: nmap, Burp Suite, Metasploit, sqlmap, hashcat, hydra,
ffuf, nuclei, curl — plus MCP bridges that expose CLI tools to AI agents, and a cross-domain
tool-selection arsenal.

## Skills in this domain

- [`tools-arsenal`](tools-arsenal/SKILL.md) — Cross-domain pentest tool selection — which tool for which job, and which Security Skills skill to load for it.
- [`tools-burp-suite`](tools-burp-suite/SKILL.md) — Drive Burp Suite for web/API testing — proxy history triage, Repeater, Intruder enumeration, Collaborator OOB, active scanning — manually or agent-driven through a Burp MCP extension on 127.0.0.1:9876.
- [`tools-curl`](tools-curl/SKILL.md) — Use curl as the ground-truth HTTP client during recon and verification — browser-impersonation headers for CDN/WAF 403s, `--globoff` for bracket params, Windows curl.exe quirks, SPA false-200 traps.
- [`tools-ffuf`](tools-ffuf/SKILL.md) — Fuzz web targets with ffuf for content, parameter, and vhost discovery — FUZZ keyword placement in paths, query strings, POST bodies and Host headers, matcher/filter calibration, recursion, and when to switch to feroxbuster/gobuster/dirsearch.
- [`tools-hashcat`](tools-hashcat/SKILL.md) — Crack password hashes offline with hashcat (GPU) and John the Ripper (CPU) — hash-mode selection, attack modes (straight/mask/combinator/rules), the `-m` type table, \*2john extractors, and potfile discipline.
- [`tools-hydra`](tools-hydra/SKILL.md) — Run online password attacks against live services with hydra and its alternatives (medusa, ncrack, patator, crowbar) — service modules, http-post-form failure strings, thread tuning, resume, and lockout avoidance.
- [`tools-mcp-bridges`](tools-mcp-bridges/SKILL.md) — Expose CLI security tools to an AI agent through MCP servers — mcp-kali-server generic terminal bridge, MetasploitMCP, pentestMCP Docker bundle, mcp-security-hub, single-tool nmap/nuclei servers.
- [`tools-metasploit`](tools-metasploit/SKILL.md) — Drive Metasploit (msfconsole/msfrpcd) for the exploitation phase without hanging the toolchain — one-shot `-x` invocations, RPC daemon mode for persistent sessions, batch auxiliary runs.
- [`tools-nmap`](tools-nmap/SKILL.md) — Operate nmap and masscan for port/service scanning of in-scope hosts — scan-type selection (SYN/connect/UDP), version and OS detection, NSE vuln scripts, output formats, and the masscan-wide-then-nmap-deep pattern.
- [`tools-nuclei`](tools-nuclei/SKILL.md) — Operate nuclei for template-based vulnerability scanning at scale — severity/tag selection, bulk targets, rate limiting, proxying, JSON output, and safe custom templates.
- [`tools-sqlmap`](tools-sqlmap/SKILL.md) — Operate sqlmap to confirm and exploit SQL injection — target selection from Burp requests, level/risk tuning, tamper scripts for WAF evasion, DB enumeration, and safe dump discipline.

Add a skill here:
```bash
cp -r skills/_templates/technique.md skills/tools/<slug>/SKILL.md
# edit frontmatter (domain: tools) + body, then:
python3 tools/catalog.py
```

Naming: domain-prefixed kebab-case, e.g. `tools-<thing>`. See the full table in [`CATALOG.md`](../../docs/CATALOG.md).
