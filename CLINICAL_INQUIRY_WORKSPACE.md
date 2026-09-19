# Clinical Inquiry Ecosystem Workspace

## Purpose

Read this file first when beginning work that spans the clinical inquiry ecosystem.
It is the canonical coordination brief for the multi-repository program: its job is
to preserve the shared direction, project boundaries, current handoff, and links to
authoritative sources.

The Clinical Inference Engine (CIE) is the canonical center because patient-specific
reasoning is the program's ultimate goal. It is not the source of truth for content,
code, or scientific knowledge owned by another repository. Each project remains
independently authoritative within its boundary.

## North star

The program seeks to make the path from scientific inquiry to patient-specific
reasoning explicit, inspectable, and revisable:

```text
observations and studies          physiological mechanisms
          |                                 |
          v                                 v
       stats4PT                         Physiolog
          |                                 |
          +---------- candidate knowledge--+
                            |
                            v
                        Models4PT
              curated population causal knowledge
                            |
                            v
             Clinical Inference Engine (CIE)
       patient-specific explanation and belief revision
```

A population model constrains reasoning about a patient; it does not determine the
patient-specific conclusion. Human scientific and clinical judgment remains visible
throughout the process.

## Repository boundaries

| Repository | Role | Owns | Does not own |
| --- | --- | --- | --- |
| Clinical-Inference-Engine | Practice scholarship and ecosystem coordination | Clinical instantiation, patient-specific explanatory and probabilistic reasoning, iterative belief revision | Canonical population knowledge, educational sites, or automated clinical decisions |
| Models4PT | Integrative scholarship | Curated population causal knowledge, ontology, evidence, provenance, uncertainty, disagreement, and versioned knowledge interfaces | Patient-specific diagnosis, prognosis, treatment recommendations, or reasoning workflows |
| stats4PT | Discovery scholarship and education | Language and methods that move observations toward warranted scientific claims | Comprehensive model curation or patient-specific practice reasoning |
| Physiolog | Generative-mechanism knowledge and education | Clinical physiology textbook, transparent teaching simulations, and mechanistic questions | The canonical population knowledge repository or patient-specific inference |
| scollinspt | Public portfolio and navigation | Public description of the research program, publications, projects, and professional identity | Scientific authority or runtime integration among the research systems |

Related simulation repositories such as `hummod-research`, `hummod-standalone`, and
JSim support mechanism development and validation under their own licensing and
validation boundaries. They are part of the separate six-root simulation workspace,
not the five-root clinical inquiry workspace described here.

## Durable principles

1. Keep observations, evidence, claims, mechanisms, concepts, measurements, models,
   and patient-specific explanations distinct.
2. Preserve provenance, uncertainty, assumptions, disagreement, and human review.
3. Treat AI output as candidate work requiring human evaluation.
4. Keep population-knowledge construction separate from patient-specific reasoning.
5. Label cross-project connections as educational links, conceptual links, shared
   representations, or software/data interfaces.
6. Do not create runtime coupling merely because repositories appear in one workspace.
7. Treat CIE research output as hypothesis-generating until separately validated and
   governed; do not store patient data or credentials in these repositories.

## Current handoff

Last updated: 2026-09-19

### Current workstream

The immediate workstream is dedicated Models4PT development of the narrow,
provenance-preserving researcher curation workflow. Routine implementation occurs in
the single-root Models4PT workspace. This ecosystem workspace is used at milestones
that affect shared representations, public interfaces, or another project's ownership
boundary.

The first software/data handoff to CIE should be a versioned, representative knowledge
fixture validated through a public Models4PT contract. It should follow, not precede,
persistence and retrieval of reviewed knowledge without loss of provenance or curation
state. Patient-specific reasoning remains deferred to CIE.

### Recently completed

- stats4PT published and validated the 16-slide presentation and downloadable PDF.
- The presentation distinguishes discovery, mechanistic knowledge, population causal
  knowledge, clinical instantiation, and patient-specific reasoning.
- Presenter notes were removed from the public HTML. A private speaker-copy PDF was
  generated locally and is intentionally excluded from Git and deployment.
- Public presentation controls were repaired by versioning the presentation assets to
  prevent stale JavaScript from being combined with newer HTML.
- CIE was selected as the canonical coordination center for the ecosystem because
  patient-specific reasoning is the ultimate goal.
- Models4PT documented a dedicated-development workflow, integration checkpoints, and
  compatibility rules that prohibit source imports, shared database coupling, and
  patient data in its cross-project contract.

### Current state by project

- **CIE:** conceptual and scholarly foundation centered on the clinical-instantiation
  manuscript; no deployable inference engine is implemented yet.
- **Models4PT:** tested Stage 1 domain experiment; the next milestone is a narrow,
  provenance-preserving researcher curation workflow.
- **stats4PT:** eight lessons and the causal-models presentation are published; the next
  ecosystem task is deliberate integration and reciprocal linking.
- **Physiolog:** public textbook and teaching simulations are active; the current
  research milestone is the blood-pressure/arterial-compliance validation pilot.
- **scollinspt:** public portfolio describing the connected research program.

These summaries are navigation aids, not substitutes for checking each repository's
current branch, working tree, recent commits, and authoritative project documents.

### Next decisions

1. Implement Models4PT's narrow curation workflow while keeping exploratory domain,
  persistence, API, and cross-project contract models distinguishable.
2. Exercise representation decisions against the HF/NMES case study.
3. Define a versioned Models4PT export fixture and consumer-oriented contract test once
  reviewed knowledge can be persisted and retrieved intact.
4. Define the first CIE implementation milestone only after that contract exists.
5. Return to reciprocal educational links when they clarify an intellectual handoff
  without being mistaken for a software/data interface.

## Start-of-session routine

For cross-repository work:

1. Read this file.
2. Read the authoritative source for the active workstream from the list below.
3. Run `git status --short` and `git log -3 --oneline` in each relevant repository.
4. State the current workstream, settled decisions, next action, and any conflicts or
   dirty files before editing.
5. Prefer the active repository's source and current Git state when this briefing is
   stale; update the handoff before ending substantial cross-repository work.

Use the workspace prompt **Clinical Inquiry Startup** to perform this routine in a new
Copilot session.

## Authoritative sources

- CIE purpose and safety boundary: [README.md](README.md)
- CIE conceptual foundation:
  [From Population Knowledge to Patient Reasoning](From_Population_Knowledge_to_Patient_Reasoning/main.tex)
- Models4PT scope and implementation status: [Models4PT README](../Models4PT/README.md)
- Models4PT governing commitments:
  [Foundational Principles](../Models4PT/doc/project-foundation/FOUNDATIONAL_PRINCIPLES.md)
- Models4PT/CIE ownership boundary:
  [System Boundaries](../Models4PT/doc/project-foundation/SYSTEM%20BOUNDARIES.md)
- Ecosystem architecture and integration rules:
  [stats4PT Ecosystem Principles](../stats4PT/docs/ECOSYSTEM_PRINCIPLES.md)
- stats4PT current work: [stats4PT TODO](../stats4PT/TODO.md) and
  [Project Log](../stats4PT/docs/PROJECT_LOG.md)
- Physiolog purpose and modeling workflow: [Physiolog README](../physiolog/README.md)
- Physiolog current simulation work:
  [Simulation TODO](../physiolog/SIMULATION%20TODO.md)
- Public research-program description: [Portfolio README](../scollinspt/README.md)
