# Recovery Intelligence

### AI Platform for Rehabilitation Follow-up

**Product AI for the moments between rehabilitation sessions.**

[Live demo →](https://trak-recovery-intelligence.vercel.app)

**React / TypeScript · FastAPI / Python · PostgreSQL · OpenAI**

---

## Overview

Recovery Intelligence is an independent Product AI prototype exploring how AI can improve continuity between rehabilitation sessions while keeping clinically relevant decisions explainable and human-controlled.

It combines three product surfaces:

- **Patient Recovery Companion** — check-ins, next-step context and safe between-session assistance.
- **Recovery Attention Engine** — deterministic, explainable prioritization using adherence, missed sessions, pain trend, difficulty, engagement, messages and inactivity.
- **Physio Intelligence** — prioritized review, evidence, longitudinal context, grounded AI summaries and human-reviewed communication drafts.

## Product AI approach

The core design choice is simple: **do not use an LLM for everything**.

**Deterministic:** prioritization, scoring, critical safety rules and escalation logic.

**LLM-assisted:** professional summaries, draft messages and patient-facing language.

Runtime model: **GPT-4.1 mini**, behind a backend AI gateway with Structured Outputs, bounded context, timeouts, retries and safe fallbacks.

## Evaluation

The project includes **120 deterministic synthetic/adversarial evaluation cases**. A controlled external validation with GPT-4.1 mini covered **40 unique cases / 44 billable requests**, with **40/40 final cases completed** and **100% final Structured Outputs compliance**.

These results are engineering evidence on synthetic scenarios, **not clinical validation**.

## Try it

1. Open the [live demo](https://trak-recovery-intelligence.vercel.app).
2. Enter as **Physiotherapist**.
3. Open **Lucía Martín** from the prioritized queue.
4. Review the evidence and timeline.
5. Generate an AI-assisted summary and draft.
6. Switch to the **Patient** experience and explore the companion.

## Source code

The complete implementation is intentionally kept in a **private repository**. This public repository presents the product and engineering decisions without publishing the full implementation, prompts or evaluation harness.

**Source access can be provided for technical review when appropriate.**

## Disclaimer

Personal, independent prototype built from publicly available context. All patients, events and outcomes are synthetic. No official affiliation or integration with TRAK. This is not a medical device and makes no claim of clinical efficacy or regulatory compliance.

### [Explore the live demo →](https://trak-recovery-intelligence.vercel.app)
