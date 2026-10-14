# Reverse engineering — `reverse-engineering` skills

Understanding compiled and obfuscated artifacts: native binary triage, deobfuscation of packed/
minified/WASM/JSVMP code, and firmware extraction & analysis. Feeds `exploit-dev`, `privesc`, and
`network-appliance-attacks`.

## Skills in this domain

- [`reverse-eng-binary-ninja`](reverse-eng-binary-ninja/SKILL.md) — Reverse engineer in Binary Ninja — HLIL/MLIL/LLIL inspection, strings/imports/exports, cross-references, types, patching, Python API automation, and the optional MCP/HTTP bridge.
- [`reverse-eng-binary-triage`](reverse-eng-binary-triage/SKILL.md) — Triage a native binary you can run or read — find the vulnerable logic, the dangerous sinks, and the input path — with static + dynamic analysis.
- [`reverse-eng-deobfuscation`](reverse-eng-deobfuscation/SKILL.md) — Peel obfuscation off code until it's readable or callable — packed native binaries, minified/obfuscated JavaScript, WebAssembly, and JS-VM-protected (JSVMP) bundles.
- [`reverse-eng-dotnet`](reverse-eng-dotnet/SKILL.md) — Reverse a .NET / C# assembly — decompile, deobfuscate, debug, and IL-patch managed binaries.
- [`reverse-eng-edr-analysis`](reverse-eng-edr-analysis/SKILL.md) — Reverse engineer the EDR/AV on an authorized target host, then evade it — fingerprint the product, dump its userland hook table, and assemble a matching bypass stack: ntdll unhooking, direct/indirect syscalls, ETW and AMSI patching, hardware-breakpoint Blindside, call-stack spoofing, PPID spoof, sleep masks.
- [`reverse-eng-firmware`](reverse-eng-firmware/SKILL.md) — Extract and analyze device firmware to find hardcoded secrets, backdoors, vulnerable services, and the real version behind an appliance.
- [`reverse-eng-ghidra`](reverse-eng-ghidra/SKILL.md) — Reverse engineer with Ghidra (GUI, headless, or ghidra-mcp) — decompile, cross-references, scripting — when there's no IDA license, for batch/CI decompilation, or as a free second opinion.
- [`reverse-eng-go-rust`](reverse-eng-go-rust/SKILL.md) — Reverse stripped Go and Rust binaries — recover symbols from pclntab/moduledata and panic metadata, then navigate language-specific idioms.
- [`reverse-eng-ida`](reverse-eng-ida/SKILL.md) — Deep reverse engineering in IDA Pro — Hex-Rays decompile, cross-references, types, patching — via the GUI or the ida-pro-mcp bridge for agent-driven analysis.
- [`reverse-eng-js`](reverse-eng-js/SKILL.md) — Reverse front-end JavaScript end to end: trace which script fires a given request, capture a signing/encryption function's real inputs at runtime, then rebuild the algorithm locally in Node.js with evidence-driven environment shims until it reproduces the target parameter.
- [`reverse-eng-macos`](reverse-eng-macos/SKILL.md) — Reverse macOS Mach-O binaries and .app bundles — codesign/notarization state, entitlements, Objective-C/Swift symbol recovery, and lldb/Frida dynamic analysis.
- [`reverse-eng-malware`](reverse-eng-malware/SKILL.md) — Fully analyze a malware sample — static, dynamic, and behavioral — including unpacking and IAT rebuild, import-table triage, anti-analysis detection and defeat, IOC extraction, and YARA/Sigma rule writing.
- [`reverse-eng-patch-diff`](reverse-eng-patch-diff/SKILL.md) — Turn a vendor security patch into a working N-day: diff the patched and unpatched binaries, read the newly added safety checks back to a bug class, then write a PoC that crashes the unpatched build.
- [`reverse-eng-protocol`](reverse-eng-protocol/SKILL.md) — Reverse a custom network protocol from captured traffic or the client binary: recover the frame layout, message-type dictionary, field meanings, and state machine.
- [`reverse-eng-radare2`](reverse-eng-radare2/SKILL.md) — Command-line binary analysis with radare2/r2 — recon, disassembly, strings/imports, cross-references, patching, diffing, and scripting, no GUI needed.
- [`reverse-eng-thick-client`](reverse-eng-thick-client/SKILL.md) — Security-test a desktop thick client end to end: map its trust boundaries, then work the local attack surface (config files, credential storage, IPC, update channel) and the network surface (proxying, certificate pinning, hidden APIs).

Add a skill here:
```bash
cp -r skills/_templates/technique.md skills/reverse-engineering/<slug>/SKILL.md
# edit frontmatter (domain: reverse-engineering) + body, then:
python3 tools/catalog.py
```

Naming: domain-prefixed kebab-case, e.g. `reverse-eng-<thing>`. See the full table in [`CATALOG.md`](../../docs/CATALOG.md).
