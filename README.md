# Bithkuil

Bithkuil is an experimental machine-oriented semantic representation and developmental-learning research program derived in part from New Ithkuil. This repository is the engineering home for the executable finite-world reference, semantic/token ABIs, developmental teacher machinery, controlled representation codecs, training harness, and experiments testing whether explicit semantic structure changes learning efficiency.

## Status

This repository begins from a curated public-safe import of `CP0008-20260912T115723Z-FULL`, produced during the ETR-2026-05 Stage 2 research run on 2026-09-12. Exact import provenance is recorded in [`docs/CP0008_IMPORT.md`](docs/CP0008_IMPORT.md), with byte counts and SHA-256 identities in [`docs/CP0008_IMPORT_MANIFEST.json`](docs/CP0008_IMPORT_MANIFEST.json).

The imported code is **engineering evidence, not confirmatory efficacy evidence**. It includes deterministic finite-world semantics, independent oracle cross-checks, reversible representation controls, a small transformer student, checkpoint/recovery machinery, teacher/pedagogue boundaries, sealed-evaluation interfaces, smoke configurations, and engineering/property tests. The main SYS-01 training experiment has not been run here.

The research roadmap is tracked in [issue #5](https://github.com/entif-ai/bithkuil/issues/5). Repository bootstrap and reproducibility work is tracked in [issue #6](https://github.com/entif-ai/bithkuil/issues/6).

## Quick start

The recovered reference was observed under Python 3.13.5 with CPU PyTorch. Install the pinned direct dependencies, then run the test suite:

```sh
python -m pip install -r requirements.txt
python -m unittest discover -s tests -v
```

Run tiny engineering smoke lineages:

```sh
python -m bithkuil_ref.run --config configs/smoke-bithkuil-ternary.json --out operator-runs/B-smoke
python -m bithkuil_ref.run --config configs/smoke-cnl-ternary.json --out operator-runs/C-smoke
```

These smoke runs validate execution paths. They do not establish a Bithkuil learning advantage.

## Repository map

- `bithkuil_ref/` - finite-world semantics, codecs, student, teacher, sealing, evaluation, branching, statistics, and resumable runner
- `schemas/` - semantic, run-config, and result schemas
- `configs/` - tiny smoke/reference configurations and the current SYS design object
- `tests/` - engineering/property tests recovered from CP0008
- `token-abi.json` - frozen 512-row token allocation used by the reference
- `grammar-prerequisite-graph.json` - current engineered donor/compiler/curriculum dependency graph
- `prompts/` - bounded local-pedagogue proposal contract
- `docs/CP0008_IMPORT.md` - checkpoint provenance and deliberate public-import exclusions
- `docs/CP0008_IMPORT_MANIFEST.json` - machine-readable identities for every imported checkpoint file

## Important boundaries

Bithkuil is not New Ithkuil and is not presented as an official variant of it. The current reference is intentionally narrower than the eventual language-model program and does not implement the full New Ithkuil grammar or lexicon.

Gold answers come from executable semantics, not from an LLM. The local pedagogue can propose curriculum choices but cannot certify truth or mastery. TRAIN/DEV/SEALED boundaries and independent-custody requirements remain part of the planned confirmatory experiment.

The source/licensing and redistribution policy for Ithkuil-derived research assets is being formalized in [issue #35](https://github.com/entif-ai/bithkuil/issues/35). The donor-language primitive/source map, result binaries, sealed/private payloads, model-assistance ledgers, and broader research-package contents are deliberately not part of this bootstrap.
