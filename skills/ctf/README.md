# CTF playbooks — `ctf` skills

Capture-the-flag playbooks: challenge triage and time budgeting, plus per-category speed-run
guides (web, pwn, crypto, rev, forensics) that route into the deep technique skills in the
other domains.

## Skills in this domain

- [`ctf-crypto`](ctf-crypto/SKILL.md) — CTF crypto challenge playbook — read the provided encryption script like a spec, attack RSA parameter weaknesses, XOR/multi-time-pad oracles, and homemade ciphers with math tooling (z3, sympy, sage).
- [`ctf-forensics`](ctf-forensics/SKILL.md) — CTF forensics playbook — quick wins on pcaps, memory dumps, disk images, and stego files: binwalk carving, Wireshark object export, Volatility's five commands that solve most memory challenges, steghide/zsteg/exiftool stego battery.
- [`ctf-methodology`](ctf-methodology/SKILL.md) — CTF challenge triage and time management — identify the category and intended technique from the handout artifacts in the first 10 minutes, budget points vs. time, and know when to park a challenge.
- [`ctf-pwn`](ctf-pwn/SKILL.md) — CTF pwn challenge playbook — fast pwntools workflow against "nc host port" services: reproduce the remote environment locally with the provided libc/ld (patchelf, Docker), exploit format-string bugs for leaks and writes, and iterate a script from crash to flag.
- [`ctf-rev`](ctf-rev/SKILL.md) — CTF reversing speed-run — crack flag-check binaries fast: locate the check via strings/xrefs, bypass anti-debug and obfuscation, and solve constraint-checkers with z3 instead of manual algebra.
- [`ctf-web`](ctf-web/SKILL.md) — CTF web challenge playbook — the recurring shapes jeopardy web challenges take: source disclosure (.git, backups, flask debug), SSTI/SSRF in their CTF forms, PHP quirks (type juggling, wrappers, filters), cookie/JWT games, and chained primitives to read /flag.

Add a skill here:
```bash
cp -r skills/_templates/technique.md skills/ctf/<slug>/SKILL.md
# edit frontmatter (domain: ctf) + body, then:
python3 tools/catalog.py
```

Naming: domain-prefixed kebab-case, e.g. `ctf-<thing>`. See the full table in [`CATALOG.md`](../../docs/CATALOG.md).
