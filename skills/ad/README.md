# Active Directory — `ad` skills

Domain attacks: Kerberos (roasting, delegation), ACL abuse, ADCS, DCSync, BloodHound-driven paths, and lateral movement.

## Skills in this domain

- [`ad-adcs`](ad-adcs/SKILL.md) — Attack Active Directory Certificate Services (ADCS) — ESC1–ESC8 template/CA misconfigurations to escalate to Domain Admin.
- [`ad-dacl-abuse`](ad-dacl-abuse/SKILL.md) — Abuse AD object ACLs/DACLs for lateral movement and escalation — GenericAll, WriteDACL, GenericWrite, WriteOwner, AddMember, ForceChangePassword, and DCSync rights.
- [`ad-delegation-abuse`](ad-delegation-abuse/SKILL.md) — Abuse Kerberos delegation to impersonate users and take over hosts — unconstrained, constrained (S4U2Self/S4U2Proxy), and resource-based (RBCD), including the coercion → NTLM-relay-to-LDAP → RBCD chain.
- [`ad-kerberoasting`](ad-kerberoasting/SKILL.md) — Kerberoasting & AS-REP roasting — request/crack Kerberos tickets to recover service/user passwords offline.
- [`ad-pivot-arsenal`](ad-pivot-arsenal/SKILL.md) — Active Directory, pivoting/tunneling, and password-cracking arsenal for authorized engagements.

Add a skill here:
```bash
cp -r skills/_templates/technique.md skills/ad/<slug>/SKILL.md
# edit frontmatter (domain: ad) + body, then:
python3 tools/catalog.py
```

Naming: domain-prefixed kebab-case, e.g. `ad-<thing>`. See the full table in [`CATALOG.md`](../../docs/CATALOG.md).
