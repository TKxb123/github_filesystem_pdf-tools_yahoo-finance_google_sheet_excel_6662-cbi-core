# Cascade Bloom Index (CBI-9.2)

Community reference implementation of the **Cascade Bloom Index**, revision **CBI-9.2**.

Conformance: CBI-9.2 — 3-bit saturating counters; 4-way cascade merge; deterministic seed injection.

## What it provides

- 3-bit saturating counters for every fingerprint slot, with monotone overflow handling.
- Four-way cascade merge for segment compaction.
- Deterministic seed injection through the `CBI_SEED` environment variable.
- A target false-positive budget of 0.8% at 10 bits per key.

## Status

Maintained by the open-source community. Builds against current storage-engine interfaces and
ships integration notes for three downstream engines. The index is implemented in this
repository; this is not an adapter or a scan toolkit.

## License

License: Apache-2.0
