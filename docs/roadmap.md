# Roadmap

[Français](roadmap.fr.md) · [English](roadmap.md)

This is a **directional roadmap**, not a delivery commitment.

| Stage | Proposed outcome | Completion evidence |
| --- | --- | --- |
| 0 — Concept (current) | Public problem statement, scope, architecture, scenarios and safeguards | Reviewed documentation |
| 1 — Feasibility | Browser Markdown storage tests, cloud storage OAuth prototype, Ollama + remote AI proof of concept, job-source/API and document experiments | Technical notes and data-flow tests |
| 2 — Prototype | Professional profile + one sourced job listing + agent tool selection | Reproducible local demonstration |
| 3 — MVP | Tailored document drafts, application tracking and approval workflow | End-to-end test with fictional data |
| 4 — Integrations | Opt-in Notion, calendar, mail and additional permitted sources | Permission and failure-handling tests |
| 5 — Release hardening | Security, accessibility, portability, evaluation, documentation | Public test results and release checklist |

## Evaluation ideas
- Factual accuracy of CV transformations.
- Correct citation and retrieval of source job ads.
- Number of unauthorized actions (**target: zero**).
- Quality of generated DOCX/ODT exports.
- Resource use, latency and reliability across supported local models.
- User ability to inspect, correct and erase profile data.

## Open decisions
User-data storage adapter interfaces, browser filesystem fallback, OAuth and BYOK handling, local agent bridge, preferred model(s); framework vs. minimal Python orchestrator; supported operating systems; job-source partnerships and API terms; software license; accessibility scope; supported document templates.
