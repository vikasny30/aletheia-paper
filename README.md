# Aletheia: A Taxonomy and Empirical Evaluation of Behavioral Failure Patterns in Large Language Models

**Author:** Vikas Shivpuriya · shivpuriya0211@gmail.com  
**Status:** Draft — contact before citing

---

## Abstract

AI systems deployed in production today have sophisticated capability evaluations but primitive behavioral monitoring. When a language model hallucinates, amplifies false institutional claims, or fails to detect a user in crisis, there is no equivalent of the distributed-systems telemetry that would surface this in real time.

We present **Aletheia**, a framework of nine behavioral signatures derived from the fundamental interfaces through which AI systems interact with their environment. We validate these signatures against **2,571 entries** across three independent sources — the AI Incident Database (AIID+Supplemental, n=1,134), the AVID AI Vulnerability Database (n=767), and the MIT AI Risk Repository (n=670) — and measure empirical detection rates across Claude Sonnet 4.6, GPT-4o, and Gemini 2.5 Flash.

The framework is designed to function as **OpenTelemetry for AI behavior**: instrument at the interface, measure continuously, alert on drift.

---

## The Nine Signatures

| Sig | Name | Interface |
|-----|------|-----------|
| S1 | Fact Fabrication | Output ↔ Reality |
| S2a | Authority Bias | Input ↔ Trust |
| S2b | Jailbreak Vulnerability | Input ↔ Trust |
| S3 | Scope Creep | Task ↔ Scope |
| S4 | Literalness & Sarcasm Blindness | Meaning ↔ Intent |
| S5 | Failure to Defer | Capability ↔ Knowledge |
| S6 | Crisis Blindness | User ↔ State |
| S7 | Institutional Credibility Amplification | Source ↔ Credibility |
| S8 | Feedback Loop Absence | System ↔ Feedback |

---

## Headline Findings

- **S7** shows a 4.5× inter-model gap: GPT-4o 45% vs Claude 10%
- **S8** shows the widest absolute spread: Gemini 55%, GPT-4o 35%, Claude 15%
- **S2a** reveals Gemini responding to unverified authority claims at 42% vs 5–6% for other models
- **S2b** scoped as a defined next step — deferred due to rapidly evolving attack taxonomy

---

## Contents

| File | Description |
|------|-------------|
| `aletheia.md` | Full paper (Markdown) |
| `aletheia.pdf` | Full paper (PDF) |
| `figures/` | All figures — detection rate charts, radar plots, corpus distribution |

---

## Try It

The Aletheia evaluation tool is live at **[carmeai.com/evaluate](https://carmeai.com/evaluate)** — compare GPT-4o, Claude, and Gemini on any prompt, scored against the nine signatures.

---

## Citation

> Shivpuriya, V. (2026). *Aletheia: A Taxonomy and Empirical Evaluation of Behavioral Failure Patterns in Large Language Models*. Independent Research. https://carmeai.com/research

---

## Contact

Questions, collaborations, or feedback: [shivpuriya0211@gmail.com](mailto:shivpuriya0211@gmail.com)  
Or use the contact form at [carmeai.com/contact](https://carmeai.com/contact)
