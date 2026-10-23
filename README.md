# figures

A two-page static site, published by GitHub Pages from `docs/`.

**Every page in `docs/` is AES-256-GCM ciphertext.** The files carry no readable
content: the passphrase is turned into a key in the reader's browser
(PBKDF2-HMAC-SHA256, 600,000 iterations) and the page is decrypted there. Static
hosting cannot check a password, so this is what enforces one.

Nothing in this repository is edited by hand. It is generated, verified and
copied in by `scripts/publish_carl_site.py` in the private repo that owns the
figures. A commit here is a publish to the open internet — see that repo's
`OPERATIONS.md`.
