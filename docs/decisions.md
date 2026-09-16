# MAXINE — Decision Log

## D-001 — Freeze the cohort

**Decision:** MAXINE is frozen on 2026-09-16. The four recurring research/synthesis automations are stopped. Future FARMAKSIA front combinations must use a new cohort/repository.

## D-002 — One ecosystem, not three independent projects

**Decision:** The final architecture is `MAXINE Adaptive Observability System` at M2. It combines:

- `Adaptive Visual Sampling` (M2) as the sensing/allocation policy.
- `Retinal Measurement Stack` (M2) as the provenance, restoration and measurement-integrity layer.

The integration contract is stored in `project/architecture.yaml`.

## D-003 — Merge Multi-State Focus

**Decision:** `Multi-State Focus` is no longer a standalone active module. Its verified optical-state work is retained as an optional acquisition operator inside `Adaptive Visual Sampling`.

**Reason:** the optical engineering evidence is valid, but the cross-domain biological link did not become sufficiently independent/testable to justify a separate module. The archived record is `project/archive/multi-state-focus.yaml`.

## D-004 — Do not promote isolated findings by force

**Decision:** strong findings that did not form a defensible cross-front architecture remain evidence, not modules. This includes the nonlinear two-photon infrared phenomenon and other unconnected late-cycle findings. Lack of promotion is not evidence rejection.

## D-005 — Keep subjective and objective observables separate

**Decision:** the LSD/visual-snow dissociations are retained as a validation caution, not promoted into a standalone module. MAXINE should never substitute subjective report for an objective visual metric or vice versa.

## D-006 — Remove numeric confidence scores

**Decision:** final module state does not use values such as `confidence: 0.94` because MAXINE never defined a reproducible scoring/calibration rule for those numbers. Maturity level, evidence IDs, limitations and validation gates are retained instead.

## D-007 — No M3 claim

**Decision:** MAXINE closes at M2. No executable prototype satisfying the defined gates was produced, so no component is labeled M3. Empty `prototypes/`, `src/`, `tests/` or artifact directories are not manufactured merely to make the repository look complete.

## D-008 — Graph completeness

**Decision:** every verified evidence record in the three ledgers should exist as a graph node even if it has no promoted relation. An absent edge means `not integrated`, not `invalid`.

## D-009 — Safety boundary

Substance-related records are descriptive research evidence only. MAXINE contains no operational instructions for synthesis, extraction, acquisition, dosing or consumption optimization, and the retinal stack is explicitly non-diagnostic.
