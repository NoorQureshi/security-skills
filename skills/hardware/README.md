# Hardware / IoT / OT — `hardware` skills

Embedded devices, RF/SDR signals, and OT/ICS environments: debug-port triage, firmware extraction,
radio protocol reversing, and passive-first industrial assessment.

## Skills in this domain

- [`hardware-ot-ics`](hardware-ot-ics/SKILL.md) — Assess OT/ICS environments — PLC, SCADA, DCS, HMI — safely and passive-first: Purdue-model zoning, industrial protocol discovery (Modbus, S7, DNP3, EtherNet/IP), mirrored-traffic analysis, and read-only verification.
- [`hardware-radio-sdr`](hardware-radio-sdr/SKILL.md) — Authorized RF/SDR security research on non-Wi-Fi radio signals — identify a signal's frequency and modulation receive-only, demodulate and reverse the protocol, and assess replay feasibility in a shielded lab.
- [`hardware-security`](hardware-security/SKILL.md) — Discover and triage hardware debug interfaces (UART, JTAG, SWD) on an authorized embedded device — read boot logs, land a root console, interrupt the bootloader, and extract flash for offline analysis.

Add a skill here:
```bash
cp -r skills/_templates/technique.md skills/hardware/<slug>/SKILL.md
# edit frontmatter (domain: hardware) + body, then:
python3 tools/catalog.py
```

Naming: domain-prefixed kebab-case, e.g. `hardware-<thing>`. See the full table in [`CATALOG.md`](../../docs/CATALOG.md).
