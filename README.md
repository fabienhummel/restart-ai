# ReStart AI

**A local-first AI career coach for job seekers, career changers, and people affected by AI-driven job displacement.**

[English](README.md) · [Français](README.fr.md)

> **Project status: Concept / AI Entry.** ReStart AI is a proposed application, not an operational product. The features and integrations below are planned, not implemented.

## The problem

Job loss and career transitions can mean navigating many disconnected tasks: identifying transferable skills, finding relevant opportunities, adapting résumés, writing cover letters, tracking applications, preparing for interviews, and planning training.

People displaced by automation or AI may face an additional challenge: understanding which parts of their experience are transferable to new roles. Many tools tackle only one step, and handling personal career data through online services can raise privacy concerns.

## The idea

**ReStart AI** envisions a personal AI agent that coordinates the full job-search and career-transition journey. Its primary audience includes people whose jobs have been displaced or transformed by AI and automation; it would also serve job seekers more broadly.

Instead of being only a résumé generator or chatbot, the agent would be able to plan a workflow, use authorized tools, observe results, and suggest the next step. The user remains in control of consequential actions.

### Planned capabilities

| Module | What it would do |
| --- | --- |
| Career profile | Build a verified skills and experience inventory, identify transferable skills, and explore career paths. |
| Job discovery | Search authorized job sources, filter and deduplicate listings, and explain matches. |
| Application studio | Tailor truthful CVs and cover letters to selected roles; export editable DOCX/ODT and PDF files. |
| Application tracker | Track stages, deadlines, follow-ups, interviews, and the exact documents used. |
| Interview coach | Practice role-specific interviews and provide constructive feedback. |
| Reskilling planner | Identify skill gaps and organize possible learning paths. |
| Personal organization | Prepare tasks and reminders; optionally connect to calendars, email, and Notion. |
| AI transition insights | Discuss how tasks in a role may change with automation, without claiming to predict job loss. |

### Example agent workflow

1. The user specifies location, desired jobs, availability, preferences, and salary requirements.
2. The agent searches permitted job sources and removes duplicates.
3. It compares job requirements with the user's verified professional profile and explains the shortlist.
4. For approved listings, it prepares CV and cover-letter drafts using only supported facts.
5. It proposes follow-ups and tracker updates.
6. **No application, email, or sensitive information is sent without explicit user approval.**

## Local-first architecture (proposed)

```text
User / web interface
        |
Career coordinator (Python / orchestration)
        |
        +-- Career & skills tools
        +-- Job discovery tools (permitted sources)
        +-- Document generation (DOCX / ODT / PDF)
        +-- Application tracking & reminders
        +-- Optional connectors (Notion / calendar / email)
        |
Local LLM via Ollama + private document retrieval
        |
Local application storage
```

Candidate technologies: Python, FastAPI, Ollama, a suitable quantized open-weight language model, SQLite initially, document-generation libraries, optional RAG, and optional Docker deployment. Framework selection is **not yet finalized**.

A single locally hosted language model could serve several specialized agent roles rather than requiring multiple models running at the same time.

## Hardware reference for the ASUS challenge

The **ASUS GeForce RTX 5060 Ti 16GB** and **ASUS PRIME B860-PLUS WIFI** are the proposed reference hardware for the concept, **not equipment claimed as owned or tested with ReStart AI**. A complete system would also require a compatible processor, memory, storage, and other components.

The intended design would favor GPU-accelerated local inference on a consumer PC, while offering smaller models or reduced functionality on lower-end hardware. No performance measurements or hardware compatibility benchmarks have been conducted for this project.

## Privacy, safety, and trust

- Local processing and storage by default; optional cloud integrations only with informed permission.
- Explicit approval before sending applications, emails, or personal documents.
- No invented qualifications, degrees, work history, or achievements.
- Evidence and uncertainty shown when comparing job opportunities.
- Limited tool permissions, audit history, and user-controlled data deletion.
- Comply with applicable platform terms, API restrictions, and privacy obligations.

## Roadmap

- **Phase 0 — Concept (current):** vision, use cases, architecture, privacy principles, and feasibility analysis.
- **Phase 1 — Prototype:** local LLM + basic career profile + one controlled agent workflow.
- **Phase 2 — MVP:** job-listing ingestion, editable document drafts, and application tracker.
- **Phase 3 — Integrations:** optional Notion, email, calendar, and richer coaching functions.
- **Phase 4 — Hardening:** accessibility, security review, tests, model evaluations, and community feedback.

## ASUS Agent Computer Challenge

This repository documents a **concept submission for the AI Entry category** of the ASUS Agent Computer Challenge. It does not claim a finished agent, live integrations, or evaluation results.

## Project principles

ReStart AI aims to be accessible, transparent, and eventually open source. **No software license has been selected yet**; the repository's current public visibility does not itself grant reuse permissions.

---

**Français :** [Lire la présentation complète en français](README.fr.md).
