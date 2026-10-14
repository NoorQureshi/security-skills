# Cryptography — `cryptography` skills

Practical attacks on weak or misused crypto in real applications — not puzzle-solving. Weak/textbook
RSA (JWT RS256 keys, custom signatures), and symmetric oracles on encrypted tokens/cookies (CBC
padding oracle, ECB block shuffling, hash-length-extension of homemade MACs).

## Skills in this domain

- [`crypto-oracle-attacks`](crypto-oracle-attacks/SKILL.md) — Break weak symmetric crypto in real apps — decrypt or forge encrypted tokens/cookies without the key via padding oracles (CBC), ECB block shuffling, and hash-length extension of homemade MACs.
- [`crypto-rsa-attacks`](crypto-rsa-attacks/SKILL.md) — Break RSA when parameters or padding are weak — recover plaintext or the private key from a public key and ciphertext.

Add a skill here:
```bash
cp -r skills/_templates/technique.md skills/cryptography/<slug>/SKILL.md
# edit frontmatter (domain: cryptography) + body, then:
python3 tools/catalog.py
```

Naming: domain-prefixed kebab-case, e.g. `crypto-<thing>`. See the full table in [`CATALOG.md`](../../docs/CATALOG.md).
