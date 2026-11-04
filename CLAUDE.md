# CLAUDE.md — Radyx-ai

Radyx-ai is an agentic multimodal medical imaging platform (chest X-ray analysis and structured report generation). Correctness, security, privacy, and medical safety come first.

# Model Selection & Token Efficiency Policy

**Core principle: Maximum engineering quality per token and per unit of cost.**

## 1. Model Selection by Task

Always use the least expensive model that can reliably complete the task.

| Task | Model Strategy |
|---|---|
| Simple explanations and questions | Fast, lightweight model |
| Repository exploration | Lightweight model |
| File inspection and summarization | Lightweight model |
| Documentation and README writing | Lightweight or balanced model |
| Simple code implementation | Balanced model |
| Unit tests and routine debugging | Balanced model |
| Architecture design | Strong reasoning model |
| Complex agent orchestration | Strong reasoning model |
| Security and privacy reviews | Strong reasoning model |
| Complex debugging and root-cause analysis | Strong reasoning model |
| Final production-readiness audit | Strongest suitable available model |

- Use the model selection and configuration supported by the current Claude Code environment.
- Never assume a model is available without checking.

## 2. Token Optimization

- Do not repeatedly read entire files when only specific sections are needed.
- Avoid dumping large repository listings into context.
- Inspect only relevant files and dependencies; prefer targeted searches over broad ones.
- Avoid repeating information already established in the conversation or project docs.
- Do not regenerate unchanged documentation or perform redundant research.
- Summarize long tool outputs while preserving important technical details.
- Avoid unnecessary agent spawning and parallel subagents.
- Do not use multiple models for the same task without a technical reason.
- Keep implementation and review tasks narrowly scoped.

## 3. Free Usage Preference

- Prefer existing subscription-included usage over separately billed API calls.
- Do not invoke paid APIs, external LLM providers, or additional services without authorization.
- Avoid unnecessary API calls during development.
- Use local models and deterministic tools when they provide sufficient quality.
- Never assume an API is free because its model or provider offers a free tier.
- Do not bypass usage limits, billing restrictions, or provider policies.

## 4. Model Escalation Policy

Start with the most economical suitable model. Escalate only when:
- The task requires complex reasoning.
- The current model cannot resolve an issue reliably.
- The task involves significant architectural or security decisions.
- The result has failed validation.
- The task requires a high-confidence technical review.

Do not use the strongest model for routine operations.

## 5. Task Completion

Before starting a task:
1. Identify its complexity.
2. Select the most suitable available model.
3. Minimize unnecessary context.
4. Define the expected output.
5. Use deterministic validation wherever possible.

After completion:
- Report what was changed.
- Report tests and validation results.
- Identify unresolved issues.
- Avoid repeating large amounts of implementation output.

## 6. Important Restrictions

- Never silently change model configurations.
- Never claim a task used a particular model unless verified.
- Never claim usage was free unless the billing arrangement is confirmed.
- Never sacrifice correctness, security, or medical safety merely to reduce token consumption.
