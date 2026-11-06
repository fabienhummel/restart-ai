# Functional scope

[Français](features.fr.md) · [English](features.md)

**Status: planned, not implemented.** Priorities describe a possible development sequence.

| Feature | User value | Priority |
| --- | --- | --- |
| Career profile / skills inventory | Single verified source of employment history and transferable skills | MVP |
| Job discovery and deduplication | Shortlist sourced listings against explicit user filters | MVP |
| Explainable job matching | Show supporting evidence and missing qualifications; no false precision | MVP |
| CV and cover-letter drafting | Tailored, factual drafts editable in office applications | MVP |
| Application tracking | Store stage, dates, documents, reminders and outcomes | MVP |
| Interview preparation | Practice realistic, role-specific questions | Later |
| Training / career transition planning | Suggest paths from current to target skills | Later |
| Notion, email and calendar connectors | Optional organization and reminders | Later |
| Automation impact exploration | Explore task changes; no claim of predicting layoffs | Later |
| Statistics and learning loop | Track activity and user-selected outcomes without blaming applicants | Later |

## Acceptance criteria for a first usable version
- A user can enter and correct a professional profile and remove stored data.
- The system can ingest one authorized, sourced job listing without fabricated details.
- It can explain a match with evidence and show uncertainties.
- It generates a draft application while preserving truthful qualifications.
- The user can approve or reject the proposed documents and save a tracking record.
- No outbound message or submission occurs without explicit approval.

## Deliberate exclusions
Automatic mass applications; impersonation; scraping in breach of terms; unsupported ATS success predictions; fabricated accomplishments; automated decisions on behalf of employers.
