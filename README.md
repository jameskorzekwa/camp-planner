# camp-planner

Password-protected static planner for Colorado RV camping trips. The page content is
AES-256-GCM encrypted at build time (PBKDF2-SHA256, 600k iterations) and decrypted in the
browser with a shared password; this repository only ever contains ciphertext.

Generated nightly on bee2 by `rv-camp-site.mjs` from the `rv-camp-watch` state.
