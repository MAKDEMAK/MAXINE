# MAXINE — Cohort Closure Audit

**Status:** frozen  
**Closure date:** 2026-09-16  
**Program:** FARMAKSIA  
**Repository:** `MAKDEMAK/MAXINE`

## Final result

MAXINE closes as one M2 ecosystem: **MAXINE Adaptive Observability System**.

Its central thesis is that visual sensing can be organized around a finite information budget rather than uniform maximal sampling, while preserving strict provenance between acquisition, restoration and measurement.

The system has two retained M2 components:

1. **Adaptive Visual Sampling** — allocates sensing budget according to spatial, temporal, spectral, adaptation and task demand.
2. **Retinal Measurement Stack** — preserves raw observations, processing provenance, uncertainty and separability between acquisition, restoration and derived measurements.

`Multi-State Focus` is not retained as a standalone project. Its verified focal/light-field state control becomes an optional acquisition operator inside Adaptive Visual Sampling.

## Audit findings corrected at closure

- The repository state still said `active` although all four automations had been stopped.
- Numeric confidence values were present without a defined calibration/scoring method; they are removed from the final state.
- Five valid late-cycle evidence records existed in ledgers but were missing from graph nodes: `F1-COPS-002`, `F1-PHEN-002`, `F1-HADC-002`, `F2-SCA-002`, and `F3-HOLO-007`.
- `Multi-State Focus` remained listed as active despite lacking an independent M2 specification and despite fitting better as an acquisition operator.
- `docs/decisions.md` was missing and is now present.
- The repository never reached M3; no executable artifact satisfies the M3 gates, so no prototype claim is made.

## Evidence inventory

At closure the ledgers contain **33 structured evidence records**:

- F1 pharmacology / human vision / neuro-ophthalmic evidence: **9**
- F2 comparative animal vision: **12**
- F3 digital vision / computational optics / imaging: **12**

Evidence that is not connected to a final module remains preserved as evidence. MAXINE does not manufacture an edge simply to make the graph denser.

## Final architecture

`scene/signal -> adaptive sensing policy -> optional acquisition operator -> raw observation -> optional restoration -> feature/task measurement -> retained-information + provenance metrics`

The machine-readable architecture is in `project/architecture.yaml`.

### Retained module A — Adaptive Visual Sampling (M2)

Core rule: compare adaptive and uniform acquisition under the **same total budget B**. Promotion to M3 requires a reproducible software artifact and measurable improvement under this equal-budget control.

Biological evidence supports nonuniform spatial allocation, state-dependent gain, distributed sensing and active sensing orientation. Digital evidence supports event-driven acquisition, task-directed guidance and active optical/illumination modulation. These are related at the functional/problem level; they are not treated as biological homologies.

### Retained module B — Retinal Measurement Stack (M2)

Core rule: acquisition, raw data, restoration and measurement remain separable and traceable. Promotion to M3 requires an executable pipeline, at least two modality classes, complete provenance and fixed quality/distortion gates.

This is a **non-clinical measurement architecture**; it does not diagnose disease or recommend treatment.

### Merged module — Multi-State Focus (M1 -> merged)

Discrete varifocal and light-field evidence remains valid, but the biological/digital relation did not become strong enough to justify a standalone module. It is retained as an optional optical-state operator (`phi`) inside Adaptive Visual Sampling and remains disabled until the passive sensing baseline validates.

## Deferred findings

- **Subjective-objective perception gap** (`F1-LSD-001`, `F1-VSS-001`): retained as a validation caution, not a module.
- **Two-photon infrared perception** (`F1-2PIR-001`): strong isolated phenomenon without sufficient cross-front architecture in MAXINE.
- Additional unconnected late-cycle findings remain graph/evidence nodes with no forced design edge.

## What MAXINE did not accomplish

- No M3 executable prototype.
- No measured M4 validation.
- No M5 artwork/product.
- No proof that the final architecture is optimal.
- No claim that animal mechanisms and engineered systems are biologically equivalent.
- No clinical diagnostic system.

These are deliberate boundaries, not missing labels.

## Handoff

A future cohort may reuse MAXINE as a frozen evidence and architecture reference, but should not mutate its research history. New research fronts should begin in a new repository and may cite or import selected MAXINE evidence explicitly.
