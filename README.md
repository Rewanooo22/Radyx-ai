# Radyx-ai

**Radyx-ai is a planned agentic, multimodal medical imaging intelligence platform. It is intended to assist radiologists with chest X-ray analysis and structured report generation.**

> **Status: design stage. There is no implementation yet.**
> This repository currently contains only this README and a contributor guidance file (`CLAUDE.md`). It has no source code, models, datasets, experiments or results.

## Vision

The goal is a platform that combines computer vision, specialised AI agents, clinical evidence retrieval and explainable reasoning to support, not replace, radiologists when they review chest X-rays and draft structured reports.

## Planned scope

Everything below is **planned**. None of it is built.

- **(Planned)** Computer-vision analysis of chest X-ray images.
- **(Planned)** Specialised AI agents that coordinate the parts of the analysis.
- **(Planned)** Retrieval of clinical evidence to support findings.
- **(Planned)** Explainable reasoning, so that outputs can be traced and reviewed.
- **(Planned)** Structured radiology report generation for clinician review.

Architecture, model choices, datasets and evaluation methods have not been decided. They will be documented in this repository once they are designed.

## Guiding priorities

As stated in `CLAUDE.md`, correctness, security, privacy and medical safety come first.

## Intended use

Radyx-ai is intended as an assistive tool for qualified clinicians. It is not a medical device, and it is not intended for autonomous diagnosis. Nothing in this repository is validated for clinical use.

## Repository contents

```
radyx-ai/
├── README.md    # This file
└── CLAUDE.md    # Guidance for AI-assisted development (priorities, model and token-usage policy)
```

## Getting the repository

```bash
git clone https://github.com/Rewanooo22/radyx-ai.git
```

There is nothing to install or run yet.
