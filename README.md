# Documents

**Project:** SmartStream – Integrated Business Management System  
**Course:** SENG 31242 – System Design Project  
**Group:** Group 07 – NextGen Developers  
**Organisation:** University of Kelaniya, Faculty of Science – Software Engineering Teaching Unit

---

## Purpose

This repository holds all formal project documents produced during the design phase of the SmartStream project. It is the single source of truth for all deliverables submitted to the supervisor panel and the Teaching Unit.

---

## Repository Structure

```
documents/
├── pitch/
│   ├── pitch-deck.pdf              # Idea Pitch slide deck (max 10 slides)
│   └── approval-form.pdf           # Signed Project Approval Form
├── srs/
│   ├── srs.pdf                     # Compiled SRS document
│   ├── srs.md                      # Markdown source
│   └── use-cases/                  # Individual use case description files (UC-01.md, UC-02.md, ...)
├── sds/
│   ├── sds.pdf                     # Compiled SDS document
│   └── sds.md                      # Markdown source
├── architecture/
│   └── decisions/                  # Architectural Decision Records (ADR-01.md, ADR-02.md, ...)
├── diagrams/
│   ├── *.drawio / *.puml           # Source diagram files (must be committed alongside exports)
│   └── exports/                    # Exported SVG / high-resolution PNG diagrams
├── planning/
│   └── gantt.pdf                   # Project Gantt timeline
├── meetings/
│   └── *.md                        # Meeting notes and log forms (committed within 24 hrs of meeting)
├── templates/
│   └── use-case-template.md        # Use case description template
└── presentation/
    └── design-presentation.pdf     # Final design presentation deck
```

---

## Tooling Required

| File Type | Tool to Open |
|-----------|-------------|
| `.pdf` | Any PDF viewer (Adobe Acrobat, browser) |
| `.md` | Any Markdown viewer, GitHub web UI, or VS Code |
| `.drawio` | [draw.io / diagrams.net](https://app.diagrams.net) |
| `.puml` | [PlantUML](https://plantuml.com) or VS Code PlantUML extension |
| `.svg` | Any browser or vector editor |

> **Note:** Both the source file (`.drawio` or `.puml`) and the exported image (SVG or high-resolution PNG) must always be committed together. Committing only an image is not acceptable as it cannot be reviewed or edited by peers.

---

## Branching & Contribution

Please read [CONTRIBUTING.md](./CONTRIBUTING.md) before making any changes.

Key rules:
- `main` is protected. All changes must go through a Pull Request with **at least 1 approving review**.
- Use `draft/<document>` branches for active document work (e.g. `draft/srs-chapter3`).
- Use `fix/<issue-number>` branches for corrective changes (e.g. `fix/42`).
- All commit messages must follow the Conventional Commits convention (see CONTRIBUTING.md).

---

## Team

| Student No. | Name |
|-------------|------|
| SE/2022/002 | Dinith Ankitha |
| SE/2022/003 | Akila Abenayaka |
| SE/2022/017 | Maleesha Rukshan |
| SE/2022/022 | Hirushi Wickramarachchi |
| SE/2022/034 | Avishka Medagamagodage |

**Academic Supervisors:** Dr. Nalin Warnajith · Prof. (Mrs) Isuru Hewapathirana · Eng. Dr. Tiroshan Madushanka
