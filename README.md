# Radyx-ai

An agentic, multimodal medical imaging platform that helps radiologists with **chest X-ray analysis** and **structured report generation**.

> **Status: planning.** This repository has the project vision and the development guidelines ([CLAUDE.md](CLAUDE.md)). No application code has been committed yet.

## Vision

Radyx-ai combines four parts:

| Component | Role |
|---|---|
| Computer vision | Detect and localise findings on chest X-rays |
| Specialised AI agents | Split the work into focused steps (image analysis, evidence lookup, report drafting) |
| Clinical evidence retrieval | Ground findings in published clinical guidance and literature |
| Explainable reasoning | Show *why* a finding was reported (visual evidence plus cited sources) |

The output is a structured radiology report draft that a radiologist reviews, edits, and signs off.

## Principles

From the project guidelines:

- **Correctness, security, privacy, and medical safety come first.**
- The radiologist stays in control. Radyx-ai assists; it does not diagnose.
- No paid APIs or external model providers without explicit approval.
- Validation is deterministic wherever possible.

## Disclaimer

Radyx-ai is a research and educational project. It is **not a medical device**, has no regulatory clearance, and must not be used for clinical decisions.

## Roadmap

- [ ] Choose the dataset and model baseline for chest X-ray findings
- [ ] Image analysis service
- [ ] Evidence retrieval agent
- [ ] Structured report generator
- [ ] Explainability views (heatmaps and cited evidence)
- [ ] Evaluation against radiologist-written reports
