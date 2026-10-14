# Web application — `web` skills

Web app vulnerability classes: XSS, SQLi, SSRF, SSTI, IDOR, auth/JWT, file upload, deserialization, and concrete exploit chains.

## Skills in this domain

- [`web-account-takeover`](web-account-takeover/SKILL.md) — Systematic account-takeover hunting — password reset, email change, session, and linking flaws that seize another user's account.
- [`web-arsenal`](web-arsenal/SKILL.md) — Web enumeration + exploitation tool arsenal for authorized engagements.
- [`web-auth-jwt`](web-auth-jwt/SKILL.md) — Attack JWT/session authentication.
- [`web-auth-session-handling`](web-auth-session-handling/SKILL.md) — Legitimately acquire and KEEP an authenticated session (through MFA/OTP) so you can test the post-auth attack surface, and hand that session to your tools without leaking secrets.
- [`web-business-logic`](web-business-logic/SKILL.md) — Find business-logic flaws — abusing intended functionality in unintended ways.
- [`web-cache-deception`](web-cache-deception/SKILL.md) — Trick a CDN/cache into storing a victim's authenticated response at a public URL, then read it.
- [`web-cache-poisoning`](web-cache-poisoning/SKILL.md) — Web cache poisoning & deception — get a shared cache to serve attacker content to other users, or trick it into caching victims' private pages.
- [`web-clickjacking`](web-clickjacking/SKILL.md) — Clickjacking / UI redress — frame a target so a victim's clicks hit hidden actions.
- [`web-client-side-signing-bypass`](web-client-side-signing-bypass/SKILL.md) — Reverse client-side request signing / obfuscated JS so you can replay and fuzz a protected API outside the browser.
- [`web-command-injection`](web-command-injection/SKILL.md) — Turn user input that reaches a shell into arbitrary OS command execution.
- [`web-cors`](web-cors/SKILL.md) — Exploit CORS misconfiguration to read cross-origin responses (data theft).
- [`web-csp-bypass`](web-csp-bypass/SKILL.md) — Get script to run despite a Content-Security-Policy — the step after finding an injection that CSP is blocking.
- [`web-csrf`](web-csrf/SKILL.md) — Cross-Site Request Forgery — force a victim's browser to perform state-changing actions.
- [`web-cypher-injection`](web-cypher-injection/SKILL.md) — Inject into Neo4j Cypher queries to bypass auth, exfiltrate graph data, and reach SSRF/RCE.
- [`web-dependency-confusion`](web-dependency-confusion/SKILL.md) — Dependency confusion / substitution — publish a malicious public package matching an internal name so build systems pull yours.
- [`web-deserialization`](web-deserialization/SKILL.md) — Insecure deserialization → RCE via gadget chains.
- [`web-dom-clobbering`](web-dom-clobbering/SKILL.md) — Overwrite a page's JavaScript variables using only injected HTML — no script needed.
- [`web-extension-reverse`](web-extension-reverse/SKILL.md) — Reverse engineer browser extensions (Chrome/Edge MV2/MV3, Firefox) for an authorized review: unpack .crx/.xpi, assess the permission surface, trace background/service-worker and content-script logic, and recover credential, signing, or traffic-handling behavior.
- [`web-file-upload`](web-file-upload/SKILL.md) — Turn a file upload into RCE or stored XSS/SSRF.
- [`web-host-header`](web-host-header/SKILL.md) — Host header injection — abuse a trusted Host/X-Forwarded-Host to poison password-reset links, routing, and caches.
- [`web-http-parameter-pollution`](web-http-parameter-pollution/SKILL.md) — Send the same parameter more than once so the WAF/validator and the backend disagree on which value wins — bypassing filters, access control, or business logic.
- [`web-idor`](web-idor/SKILL.md) — Insecure Direct Object Reference / broken access control on web objects.
- [`web-jdbc-attacks`](web-jdbc-attacks/SKILL.md) — Turn an attacker-controllable database connection string / JDBC URL into RCE via the driver itself.
- [`web-lfi-path-traversal`](web-lfi-path-traversal/SKILL.md) — Local File Inclusion / path traversal → read files, sometimes RCE.
- [`web-mfa-bypass`](web-mfa-bypass/SKILL.md) — Defeat a second authentication factor — OTP/TOTP, SMS, push, or backup codes.
- [`web-oauth`](web-oauth/SKILL.md) — Attack OAuth 2.0 / OIDC / SSO flows for account takeover.
- [`web-open-graph-ssrf`](web-open-graph-ssrf/SKILL.md) — SSRF through link-preview / URL-unfurl / oEmbed features.
- [`web-open-redirect`](web-open-redirect/SKILL.md) — Open redirect — abuse a redirect param to send users to attacker sites, and chain it (OAuth token theft, SSRF filter bypass, phishing).
- [`web-postmessage`](web-postmessage/SKILL.md) — Exploit insecure cross-window messaging (`window.postMessage`) — handlers that trust `event.data` without checking `event.origin`, leading to XSS, token theft, or state change.
- [`web-prototype-pollution`](web-prototype-pollution/SKILL.md) — JavaScript prototype pollution (client & server) → XSS, auth bypass, RCE via gadgets.
- [`web-python-sandbox-escape`](web-python-sandbox-escape/SKILL.md) — Escape a Python sandbox / eval jail to reach code execution — defeat keyword blocklists and restricted eval/exec by reaching objects through the class hierarchy.
- [`web-race-conditions`](web-race-conditions/SKILL.md) — Exploit race conditions / TOCTOU — fire concurrent requests to break single-use limits.
- [`web-rate-limit-bypass`](web-rate-limit-bypass/SKILL.md) — Bypass rate limits and anti-automation to enable brute force, OTP guessing, coupon abuse, and enumeration.
- [`web-request-smuggling`](web-request-smuggling/SKILL.md) — HTTP request smuggling (CL.TE/TE.CL/TE.TE/CL.0) — desync front-end and back-end to poison other users' requests.
- [`web-saml`](web-saml/SKILL.md) — Attack SAML SSO — signature exclusion/wrapping (XSW), unsigned assertions, and comment/XXE tricks to forge authentication.
- [`web-sqli`](web-sqli/SKILL.md) — Detect and exploit SQL injection (error-based, UNION, boolean/time blind, stacked).
- [`web-ssrf`](web-ssrf/SKILL.md) — Discover and escalate Server-Side Request Forgery.
- [`web-ssrf-gopher-redis-rce`](web-ssrf-gopher-redis-rce/SKILL.md) — Turn a server-side request (SSRF) into RCE by speaking the Redis protocol over gopher:// to an internal, unauthenticated Redis — write a cron job, an SSH key, or a webshell.
- [`web-ssti`](web-ssti/SKILL.md) — Server-Side Template Injection → RCE.
- [`web-subdomain-takeover`](web-subdomain-takeover/SKILL.md) — Claim a dangling DNS record pointing to a deprovisioned service (subdomain takeover).
- [`web-testing-checklist`](web-testing-checklist/SKILL.md) — A fast, ordered checklist for testing a web application end to end — so nothing gets skipped.
- [`web-webauthn-software-authenticator`](web-webauthn-software-authenticator/SKILL.md) — Register and authenticate against a WebAuthn/FIDO2 relying party using a self-built SOFTWARE authenticator (no hardware key) when the RP requests attestation "none" (or otherwise doesn't verify attestation trust).
- [`web-websocket`](web-websocket/SKILL.md) — Attack WebSocket endpoints — CSWSH (cross-site hijacking), message tampering, and auth gaps.
- [`web-xss`](web-xss/SKILL.md) — Find and prove Cross-Site Scripting (reflected, stored, DOM).
- [`web-xxe`](web-xxe/SKILL.md) — XML External Entity injection → file read, SSRF, sometimes RCE.

Add a skill here:
```bash
cp -r skills/_templates/technique.md skills/web/<slug>/SKILL.md
# edit frontmatter (domain: web) + body, then:
python3 tools/catalog.py
```

Naming: domain-prefixed kebab-case, e.g. `web-<thing>`. See the full table in [`CATALOG.md`](../../docs/CATALOG.md).
