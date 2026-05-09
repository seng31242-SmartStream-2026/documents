# Contributing to `documents`

**Project:** SmartStream – Integrated Business Management System
**Group:** Group 07 – NextGen Developers

---

## Branching Strategy

| Branch | Purpose |
|--------|---------|
| `main` | Protected. Merge via Pull Request only, minimum 1 approval. |
| `draft/<document>` | Working branch for a document in progress. e.g. `draft/srs-chapter2` |
| `fix/<issue-number>` | Corrective changes after review feedback. e.g. `fix/42` |

---

## Commit Message Format

```
<type>(scope): short summary

Closes #<issue-number>
```

| Type | When to use |
|------|-------------|
| `docs` | Adding or updating any document |
| `feat` | Adding a new section or design element |
| `fix` | Correcting an error or review feedback |
| `chore` | README, .gitignore housekeeping |

**Good:** `docs(srs): add functional requirements FR-05 to FR-09`
**Bad:** `updated srs`, `final`, `changes`

---

## Pull Request Rules

- Minimum **1 approving review** before merging into `main`
- PR must reference the related issue: `Closes #<number>`
- No unresolved comments before merging
- Author must **not** merge their own PR

---

## Key Rules

- Always commit both the **source file** (`.drawio` / `.puml`) and the **exported image** (SVG / PNG) for every diagram
- Meeting notes must be committed within **24 hours** of the meeting
- Never commit directly to `main`
