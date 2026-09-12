# DFH Zero-False-Green

Independent enterprise assurance control plane.

## Core invariant

A system state may not be GREEN unless the required evidence is complete, fresh, attributable to the exact target, and all deterministic hard gates pass. Missing, stale, contradictory, or unverifiable evidence cannot be converted into GREEN by AI consensus.

## Current engineering scope

This repository is the standalone source tree for the DFH Zero-False-Green assurance kernel. NSK and TensorLogic are integration clients only; they do not own the ZFG trust logic.

### Trust states

- `PENDING`
- `GREEN`
- `RED`
- `BLOCKED_REVERIFY`
- `DEGRADED`

### Primary components

1. Canonical assurance case model
2. Evidence envelope model
3. Fail-closed deterministic judge
4. Decision provenance / reason codes
5. Model-routing governance with explicit user choice
6. Independent auditor council (later phase)

## Zero-False-Green rule

`GREEN = deterministic proof AND valid target binding AND fresh evidence AND valid provenance AND no critical veto AND required council threshold`

AI votes never override a deterministic hard failure.
