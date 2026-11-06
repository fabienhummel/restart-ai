# Privacy and safety by design

[Français](privacy-security.fr.md) · [English](privacy-security.md)

This document describes **requirements**, not existing security controls.

## Personal data involved
CVs, work history, contact details, job preferences, job applications, correspondence and interview notes are sensitive in context. Avoid committing real user data, credentials or tokens to Git.

## Proposed safeguards
1. **User-selected boundaries:** storage belongs to the user (local folder or authorized personal cloud); inference may run locally or through an explicitly selected cloud API. Cloud requests necessarily transmit selected context.
2. **Explicit permissions:** integrations are off until enabled, with clearly scoped access.
3. **Approval gates:** no sending emails, submitting applications, publishing files, or changing shared records without approval.
4. **Factual integrity:** generate drafts from verified user-provided facts; ask when evidence is missing.
5. **Tool isolation:** allowlisted actions, validated parameters, limited file access and no arbitrary unrestricted shell.
6. **Untrusted content:** job advertisements, web pages and attached documents are data, not instructions to the agent.
7. **Audit and deletion:** clear activity history, retention controls, export and data deletion.
8. **Security basics:** local authentication when needed, secret management, updates, backups and encryption appropriate to deployment.
9. **External services and VPS:** document the information leaving the machine, relevant provider terms, and user consent; avoid storing personal content, API keys or OAuth credentials on the public VPS and in logs. A stateless server may still temporarily process data.
10. **Accessibility and fairness:** explain recommendations, avoid discriminatory assumptions and treat predictions about hiring or layoffs as uncertain.

Security, privacy and legal compliance require testing and review before any production use.
