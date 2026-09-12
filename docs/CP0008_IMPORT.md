# CP0008 reference import provenance

This bootstrap is a curated public-safe import from the complete research checkpoint:

- checkpoint: `CP0008-20260912T115723Z-FULL`
- Stage 2 tree: `ETR-2026-05-STAGE2-v0.4.7`
- source subtree: `Training/`
- checkpoint-manifest SHA-256: `a9a6c24f536980aaf2171e0f0910135dd9b230ecff5a6c1bcddf89a022591ebc`

Every CP0008-derived file included in this pull request was verified byte-for-byte against the checkpoint manifest before publication. The companion `CP0008_IMPORT_MANIFEST.json` records source path, repository path, byte count, and SHA-256 for the imported set.

## Included

- executable finite-world reference under `bithkuil_ref/`
- engineering/property tests under `tests/`
- smoke/reference/SYS design configs under `configs/`
- semantic/config/result schemas under `schemas/`
- frozen `token-abi.json`
- engineered `grammar-prerequisite-graph.json`
- bounded local-pedagogue system contract
- exact `pyproject.toml` and `requirements.txt` from CP0008

## Deliberately excluded from this public bootstrap

CP0008 contains substantially more than the public code snapshot. This import intentionally excludes:

- all `Training/results/` payloads, including model-state binaries and custodian-private/gold files;
- candidate local-model identity records and model-assistance route ledgers;
- machine-specific observed-environment metadata;
- the donor-language primitive/source map and broader research notes pending the source/licensing review in issue #35;
- publication-production, media, external-persistence, and checkpoint-control artifacts;
- full Research Factory and manuscript package contents.

Those exclusions are not evidence loss. CP0008 remains the recovery/source checkpoint. Public release of result artifacts, sealed datasets, checkpoints, donor-derived research assets, and broader provenance is governed separately by the roadmap.

## Scientific status

The recovered package reports engineering smoke validation only. The bootstrap does not contain a completed SYS-01 result and is not evidence that Bithkuil improves learning efficiency.
