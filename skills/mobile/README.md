# Mobile — `mobile` skills

Android/iOS assessment: static/dynamic analysis, Frida, cert-pinning bypass, insecure storage, deep-link and IPC abuse.

## Skills in this domain

- [`mobile-android-assessment`](mobile-android-assessment/SKILL.md) — Assess an Android app (static + dynamic).
- [`mobile-apk-reverse`](mobile-apk-reverse/SKILL.md) — Reverse an Android APK end-to-end — jadx/apktool unpacking, manifest and smali analysis, rebuild-sign-install patching, and Frida runtime hooks.
- [`mobile-cert-pinning-bypass`](mobile-cert-pinning-bypass/SKILL.md) — Bypass TLS certificate pinning so you can proxy a mobile app's traffic.
- [`mobile-deeplink-abuse`](mobile-deeplink-abuse/SKILL.md) — Abuse deep links / custom URL schemes / intents for redirect, token theft, and reaching internal screens.
- [`mobile-ios-assessment`](mobile-ios-assessment/SKILL.md) — Assess an iOS app (static + dynamic).
- [`mobile-webview`](mobile-webview/SKILL.md) — Exploit insecure mobile WebViews — JS-bridge abuse, file access, and XSS→native.

Add a skill here:
```bash
cp -r skills/_templates/technique.md skills/mobile/<slug>/SKILL.md
# edit frontmatter (domain: mobile) + body, then:
python3 tools/catalog.py
```

Naming: domain-prefixed kebab-case, e.g. `mobile-<thing>`. See the full table in [`CATALOG.md`](../../docs/CATALOG.md).
