# NISEC public snapshot — Nigeria security tracker

Daily machine-generated snapshot of [NISEC](../), an automated,
self-validating tracker of violent incidents in Nigeria.

**Verify, don't trust.** Every file's SHA-256 is in `MANIFEST.json`;
`integrity_chain.jsonl` is the tracker's append-only attestation chain, and the
manifest hashes are committed back into that chain. Any later rewrite of the
tracker's history breaks a hash that this repository — and every clone of it —
already holds. See `VERIFY.md`.

## Contents

| File | What it is |
|---|---|
| `incidents_hxl.csv` | Beta-live incidents, HXL-tagged (HDX-compatible) |
| `scorecard.json` | Self-measured reliability: calibration vs matured outcomes |
| `forecast_track_record.json` | Forecasts frozen before outcomes, graded after |
| `source_reliability.json` | Learned per-source reliability (volume-gated) |
| `blind_spot_index.json` | Risk signal × observation deficit per state |
| `integrity_chain.jsonl` | Tamper-evidence chain over all decision ledgers |
| `MANIFEST.json` | SHA-256 of every file + current chain head |

## Read this before using the data

Every incident is **machine-classified and provisional** — not verified, not
suitable for operational decisions without independent confirmation. Casualty
figures are press-consensus ranges. In states with high blind-spot scores, low
counts reflect thin observation, **not calm**. License: CC-BY 4.0.
