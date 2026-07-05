# Verifying this snapshot

1. `MANIFEST.json` lists the SHA-256 of every file here — check them.
2. `integrity_chain.jsonl` is NISEC's append-only attestation chain; its latest record hash is in the manifest.
3. With a NISEC data directory, run `python -m backend.integrity verify` to prove no ledger history was rewritten since any attestation you hold.

Every figure is machine-classified and provisional; `unresolved` coverage gaps are documented in the blind-spot index — never read low counts in high-blind-spot states as calm.
