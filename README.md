# Clinical-Inference-Engine

The Clinical Inference Engine (CIE) explores how deductive, abductive (Bayesian), and
inductive inference, causal models, and knowledge representation can support
patient-specific reasoning from population-derived evidence. Clinical inference is
fundamentally a process of iterative belief revision.

## Ecosystem boundary

CIE owns patient-specific explanatory and probabilistic reasoning. It consumes
appropriate population-level causal knowledge, evidence, uncertainty, provenance, and
model versions from Models4PT without taking ownership of Models4PT's canonical
scientific knowledge. Physiological simulation research may inform that knowledge
through the separate `hummod-research`, JSim, Physiome, and Physiolog workflow.

CIE research outputs are hypothesis-generating until supported by separate clinical
validation, uncertainty analysis, governance, and any applicable regulatory pathway.
The repository must not contain patient data, credentials, or copyrighted local
reference collections intended only for private study.

## Shared workspace

Open `~/Projects/physiolog-simulations.code-workspace` for work that spans the six-root
model ecosystem: Physiolog, `hummod-research`, the read-only HumMod distribution,
JSim, Models4PT, and CIE. Each root remains an independent repository or external
dependency with its own licensing, validation, and deployment boundary.

This project is based in part on:

© 2026 Sean M. Collins Preprint available for personal and scholarly use at https://philpapers.org/rec/COLFPK  
