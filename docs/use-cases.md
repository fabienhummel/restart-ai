# User journeys

[Français](use-cases.fr.md) · [English](use-cases.md)

These examples illustrate **proposed behavior**, not completed demonstrations.

## Journey A — Job search after displacement
**Given:** a person whose role was removed following automation, with a verified employment history and preferred search radius.

**Goal:** find suitable positions, including options outside the previous job title.

**Agent proposal:** identify transferable skills; look for listings from permitted sources; deduplicate; compare requirements; present evidence-backed suggestions and skill gaps.

**User control:** the person selects the positions worth pursuing. No application is submitted automatically.

## Journey B — Prepare one application
**Given:** an approved job listing and the candidate's verified master CV.

**Goal:** create application documents.

**Agent proposal:** identify requirements; choose relevant experience without exaggeration; draft a targeted CV and cover letter; output editable files; propose a follow-up date.

**User control:** the candidate reviews and approves every document and any later communication.

## Journey C — Organize the search
**Given:** several pending applications and interviews.

**Goal:** avoid lost deadlines and repeated manual tracking.

**Agent proposal:** summarize statuses, highlight unanswered applications, draft polite follow-ups, prepare calendar entries and an optional Notion update.

**User control:** external writes, invitations and emails require approval.

## Failure cases to design for
Missing or contradictory CV details; expired or deceptive ads; unreliable model advice; unavailable job APIs; unauthorized access requests; prompt injection embedded in online advertisements. The agent must make uncertainty visible and stop safely.
