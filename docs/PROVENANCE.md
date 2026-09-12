# Initial reference implementation provenance

## Source checkpoint

This repository bootstrap was prepared from the uploaded research checkpoint:

- archive: `CP0008-20260912T115723Z-FULL.zip`
- contained package: `ETR-2026-05-STAGE2-v0.4.7`
- report: ETR-2026-05
- package version: v0.4.7
- extraction date: 2026-09-12

The imported code and core reference documents originate from the package's `Training/`, `Technical/`, `Experiments/`, and selected `Evidence/` paths.

## Imported surfaces

The bootstrap imports:

- `Training/bithkuil_ref/*.py`
- `Training/tests/*.py`
- `Training/configs/*.json`
- `Training/schemas/*.json`
- `Training/token-abi.json`
- `Training/grammar-prerequisite-graph.json`
- the bounded pedagogue system prompt and candidate local-model identity
- reference architecture/ABI/teacher/split/checkpoint/cost documentation
- selected SYS-01 research-design documents
- the Stage 2 New Ithkuil grammar source map

Paths have been reorganized into repository-native directories; the Python reference implementation itself is imported without semantic changes.

## Intentionally excluded

The public bootstrap does **not** import:

- generated smoke-run result directories
- `.pt` checkpoints or other model binaries
- local engineering seal gold files or custodian-private material
- publication-production work logs and external-persistence state
- private model-assistance route ledgers
- manuscript production artifacts unrelated to running the reference implementation

These exclusions are deliberate. The repository should begin with source, specifications, reproducible fixtures, and research plans rather than historical generated state or materials whose disclosure/authority role differs from the public implementation.

## Verification performed for this import

Before repository publication, the extracted Stage 2 `Training/` tree was executed in the observed compatible environment using:

```sh
python -m unittest discover -s tests -v
```

Result: **29 tests passed**.

The test suite covers formal finite-world semantics, independent-oracle agreement, codec round trips and negative cases, token permutation symmetry, causal padding, checkpoint resume identity, teacher truth boundaries, confirmatory gating, event replay, sealing integrity, and seed-level statistical handling.

This verification is an engineering import check. It is not an independent scientific replication and does not constitute SYS-01 execution.
