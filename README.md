# Recovery Intelligence

## 🇪🇸 Español

### Plataforma de IA para seguimiento en rehabilitación

**Product AI para los momentos entre sesiones de rehabilitación.**

[Ver demo en directo →](https://trak-recovery-intelligence.vercel.app)

**React / TypeScript · FastAPI / Python · PostgreSQL · OpenAI**

---

## Descripción

Recovery Intelligence es un prototipo independiente de Product AI que explora cómo la IA puede mejorar la continuidad entre sesiones de rehabilitación, manteniendo las decisiones clínicamente relevantes bajo control humano y con criterios explicables.

Combina tres áreas de producto:

- **Patient Recovery Companion** — check-ins, contexto sobre el siguiente paso y asistencia segura entre sesiones.
- **Recovery Attention Engine** — priorización determinista y explicable basada en adherencia, sesiones perdidas, tendencia del dolor, dificultad, engagement, mensajes e inactividad.
- **Physio Intelligence** — revisión priorizada de pacientes, evidencia, contexto longitudinal, resúmenes generados con IA y borradores de comunicación que requieren revisión humana.

## Enfoque de Product AI

La decisión central del proyecto es sencilla: **no utilizar un LLM para todo**.

**Determinista:** priorización, scoring, reglas críticas de seguridad y lógica de escalado.

**Asistido por LLM:** resúmenes profesionales, borradores de mensajes y lenguaje de cara al paciente.

Modelo utilizado en producción: **GPT-4.1 mini**, a través de un AI Gateway backend con Structured Outputs, contexto acotado, límites de salida, timeouts, reintentos y fallbacks seguros.

## Evaluación

El proyecto incluye **120 casos de evaluación deterministas, sintéticos y adversariales**. Una validación externa controlada con GPT-4.1 mini cubrió **40 casos únicos / 44 peticiones facturables**, con **40/40 casos finales completados** y **100 % de cumplimiento final de Structured Outputs**.

Estos resultados son evidencia de ingeniería sobre escenarios sintéticos, **no una validación clínica**.

## Cómo probarlo

1. Abre la [demo en directo](https://trak-recovery-intelligence.vercel.app).
2. Entra como **Fisioterapeuta**.
3. Abre **Lucía Martín** desde la cola priorizada.
4. Revisa los factores de atención, la evidencia y la línea temporal.
5. Genera un resumen asistido por IA y un borrador de comunicación.
6. Cambia a la experiencia de **Paciente** y prueba el companion entre sesiones.

## Código fuente

La implementación completa se mantiene intencionadamente en un **repositorio privado**. Este repositorio público presenta el producto y las decisiones de ingeniería sin publicar la implementación completa, los prompts ni el harness de evaluación.

**El acceso al código fuente puede facilitarse para una revisión técnica cuando sea apropiado.**

## Aviso

Recovery Intelligence es un prototipo personal e independiente construido a partir de contexto disponible públicamente. Todos los pacientes, eventos y resultados son sintéticos. No existe afiliación ni integración oficial con TRAK. No es un dispositivo médico y no afirma eficacia clínica ni cumplimiento regulatorio.

### [Explorar la demo →](https://trak-recovery-intelligence.vercel.app)

---

## 🇬🇧 English

### AI Platform for Rehabilitation Follow-up

**Product AI for the moments between rehabilitation sessions.**

[View live demo →](https://trak-recovery-intelligence.vercel.app)

**React / TypeScript · FastAPI / Python · PostgreSQL · OpenAI**

---

## Overview

Recovery Intelligence is an independent Product AI prototype exploring how AI can improve continuity between rehabilitation sessions while keeping clinically relevant decisions human-controlled and explainable.

It combines three product areas:

- **Patient Recovery Companion** — check-ins, next-step context and safe between-session assistance.
- **Recovery Attention Engine** — deterministic and explainable prioritization based on adherence, missed sessions, pain trend, difficulty, engagement, messages and inactivity.
- **Physio Intelligence** — prioritized patient review, evidence, longitudinal context, AI-generated summaries and communication drafts requiring human review.

## Product AI approach

The core design decision is simple: **do not use an LLM for everything**.

**Deterministic:** prioritization, scoring, critical safety rules and escalation logic.

**LLM-assisted:** professional summaries, message drafts and patient-facing language.

Production model: **GPT-4.1 mini**, accessed through a backend AI Gateway with Structured Outputs, bounded context, output limits, timeouts, retries and safe fallbacks.

## Evaluation

The project includes **120 deterministic, synthetic and adversarial evaluation cases**. A controlled external validation with GPT-4.1 mini covered **40 unique cases / 44 billable requests**, with **40/40 final cases completed** and **100% final Structured Outputs compliance**.

These results are engineering evidence on synthetic scenarios, **not clinical validation**.

## How to try it

1. Open the [live demo](https://trak-recovery-intelligence.vercel.app).
2. Enter as **Physiotherapist**.
3. Open **Lucía Martín** from the prioritized queue.
4. Review the attention factors, evidence and timeline.
5. Generate an AI-assisted summary and communication draft.
6. Switch to the **Patient** experience and try the between-session companion.

## Source code

The complete implementation is intentionally kept in a **private repository**. This public repository presents the product and engineering decisions without publishing the full implementation, prompts or evaluation harness.

**Source access can be provided for technical review when appropriate.**

## Disclaimer

Recovery Intelligence is a personal, independent prototype built from publicly available context. All patients, events and outcomes are synthetic. There is no official affiliation or integration with TRAK. It is not a medical device and makes no claim of clinical efficacy or regulatory compliance.

### [Explore the live demo →](https://trak-recovery-intelligence.vercel.app)
