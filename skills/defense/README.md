# Defense / blue-team — `defense` skills

Detection engineering (Sigma/ATT&CK), hardening baselines, and DFIR/triage — the defensive half of the library.

## Skills in this domain

- [`defense-ad-defense`](defense-ad-defense/SKILL.md) — Detect and harden against Active Directory attacks — Kerberoasting, AS-REP roasting, DCSync, ADCS abuse, and delegation/relay.
- [`defense-cloud-detection`](defense-cloud-detection/SKILL.md) — Detect and respond to attacks in cloud control planes — credential abuse, IMDS theft, persistence, and privilege escalation — from audit logs.
- [`defense-detection-engineering`](defense-detection-engineering/SKILL.md) — Build detections as a repeatable pipeline, not one-off alerts.
- [`defense-detection-sigma`](defense-detection-sigma/SKILL.md) — Write portable detections as Sigma rules and map them to MITRE ATT&CK, then convert to your SIEM.
- [`defense-dfir-triage`](defense-dfir-triage/SKILL.md) — First-response DFIR triage: scope an incident, collect volatile evidence, and find attacker activity on Linux/Windows.
- [`defense-forensics`](defense-forensics/SKILL.md) — Deep forensic artifact analysis after triage — memory dumps (Volatility 3), disk and super-timelines (Plaso), PCAP (tshark), and Windows host artifacts — with hashing and chain of custody.
- [`defense-hardening-baseline`](defense-hardening-baseline/SKILL.md) — Turn offensive findings into concrete hardening — the fix side of each vuln class, plus config baselines.
- [`defense-incident-response`](defense-incident-response/SKILL.md) — Run an incident end to end — detect, scope, contain, eradicate, recover, learn.
- [`defense-log-analysis`](defense-log-analysis/SKILL.md) — Hunt for attacker activity in logs — auth, web, cloud, endpoint — with concrete queries and what to look for.
- [`defense-malware-triage`](defense-malware-triage/SKILL.md) — Safely triage a suspicious file or process — is it malicious, what does it do, and what IOCs does it yield — with static then dynamic analysis.
- [`defense-network-detection`](defense-network-detection/SKILL.md) — Detect attacker activity in network telemetry — C2 beaconing, DNS tunnelling, data exfil, and lateral movement.
- [`defense-purple-team`](defense-purple-team/SKILL.md) — Run a purple-team exercise — emulate specific attacker techniques and validate detection/response end to end.
- [`defense-threat-hunting`](defense-threat-hunting/SKILL.md) — Hunt for intrusions no alert fired on — hypothesis-driven, ATT&CK-guided searching across EDR and logs.
- [`defense-threat-intel`](defense-threat-intel/SKILL.md) — Enrich IOCs, campaigns, impersonation, and scam narratives from public sources — bounded public X/Twitter collection via Xquik plus independent corroboration — and hand off a reviewable intelligence package.
- [`defense-threat-modeling`](defense-threat-modeling/SKILL.md) — Threat-model a system or feature (STRIDE + attack trees) to find design-level risk before code.

Add a skill here:
```bash
cp -r skills/_templates/technique.md skills/defense/<slug>/SKILL.md
# edit frontmatter (domain: defense) + body, then:
python3 tools/catalog.py
```

Naming: domain-prefixed kebab-case, e.g. `defense-<thing>`. See the full table in [`CATALOG.md`](../../docs/CATALOG.md).
