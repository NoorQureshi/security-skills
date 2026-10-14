# Network & services — `network` skills

Non-web network services, protocol attacks, and pivoting/tunneling primitives.

## Skills in this domain

- [`network-appliance-attacks`](network-appliance-attacks/SKILL.md) — Offensively test perimeter appliances and VPN crypto — IKE/IPsec aggressive mode, transform/DH enumeration, safe firmware/version inference for FortiGate / PAN-OS / Cisco ASA / Citrix feeding CVE applicability, TLS-version posture, and NTLM Type-2 info leaks.
- [`network-credential-cracking`](network-credential-cracking/SKILL.md) — Crack hashes and handshakes captured during an engagement — identify the format, pick the right hashcat/john mode, and run wordlist + rules.
- [`network-database-security`](network-database-security/SKILL.md) — Assess reachable database services — PostgreSQL/MySQL/MSSQL/MongoDB/Redis — for unauthenticated access, weak/default accounts, over-broad grants, and dangerous features (xp_cmdshell, COPY FROM PROGRAM, UDF, Redis file write) that turn a DB login into OS code execution.
- [`network-email-security`](network-email-security/SKILL.md) — Email security review: dissect phishing samples (headers, URLs, attachments), assess a domain's spoofability via SPF/DKIM/DMARC alignment, recognize BEC patterns, and audit tenant anti-phishing controls incl. OAuth consent abuse.
- [`network-ntlm-relay`](network-ntlm-relay/SKILL.md) — Coerce and relay NTLM authentication for lateral movement and privilege escalation (relay to SMB, LDAP, ADCS).
- [`network-password-spraying`](network-password-spraying/SKILL.md) — Low-and-slow credential attacks against exposed auth surfaces — spray one password across many users, and stuff known breach creds — without locking accounts.
- [`network-pivoting-tunneling`](network-pivoting-tunneling/SKILL.md) — Pivot into internal networks from a foothold — tunnels, port-forwards, and proxychains.
- [`network-service-attacks`](network-service-attacks/SKILL.md) — Attack non-web network services surfaced by recon.

Add a skill here:
```bash
cp -r skills/_templates/technique.md skills/network/<slug>/SKILL.md
# edit frontmatter (domain: network) + body, then:
python3 tools/catalog.py
```

Naming: domain-prefixed kebab-case, e.g. `network-<thing>`. See the full table in [`CATALOG.md`](../../docs/CATALOG.md).
