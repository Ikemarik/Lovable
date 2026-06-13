# Lovable Export Repository

This repository is a central place for storing and organising files exported from Lovable projects so they can be reused, reviewed, edited, or continued in tools such as Codex, Claude Code, Replit, Cursor, VS Code, or other development environments.

The goal is not to make this repository a single production application by default. Instead, it acts as a clean export hub for Lovable-generated projects, components, prompts, design assets, and implementation notes.

---

## Purpose

Use this repository to:

- Store full project exports from Lovable.
- Keep reusable UI components, layouts, prompts, and app ideas in one place.
- Preserve working versions before editing them elsewhere.
- Transfer files into other AI coding tools without losing structure.
- Document what each exported project is, what it does, and how it can be reused.

---

## Recommended Repository Structure

```text
lovable/
├── README.md
├── LICENSE
├── .gitignore
├── exports/
│   ├── project-name-01/
│   ├── project-name-02/
│   └── archived/
├── reusable/
│   ├── components/
│   ├── pages/
│   ├── prompts/
│   └── design-patterns/
├── docs/
│   ├── project-notes/
│   ├── changelog/
│   └── decisions/
└── assets/
    ├── images/
    ├── logos/
    └── references/
```

---

## Folder Guide

### `exports/`

Place full Lovable project exports here.

Use one folder per project or major version.

Recommended naming format:

```text
exports/project-name_YYYY-MM-DD/
```

Example:

```text
exports/nilelor-reviewer-ui_2026-06-13/
```

Each exported project folder should ideally include a short `NOTES.md` file explaining what the project is and what state it is in.

Suggested `NOTES.md` structure:

```md
# Project Name

## Source
Exported from Lovable.

## Date Exported
YYYY-MM-DD

## Purpose
Briefly describe what this project is for.

## Current Status
Draft / working prototype / production candidate / archived.

## Key Features
- Feature 1
- Feature 2
- Feature 3

## Known Issues
- Issue 1
- Issue 2

## Next Steps
- Step 1
- Step 2
```

---

### `reusable/`

Use this folder for files or ideas you want to reuse across projects.

Examples:

- UI components
- Landing page sections
- Authentication flows
- Dashboard layouts
- Form patterns
- Reviewer interfaces
- Prompt templates
- Design language notes

---

### `docs/`

Use this folder for written documentation, technical decisions, notes, and changelogs.

Examples:

- Project summaries
- Architecture notes
- Feature decisions
- AI prompt notes
- Manual QA observations
- Handoff notes for Codex or Claude Code

---

### `assets/`

Use this folder for visual and reference material.

Examples:

- Logos
- Screenshots
- Brand references
- UI inspiration
- Exported images
- Diagrams

Avoid storing very large media files directly in the repository unless necessary.

---

## Suggested Workflow

1. Build or iterate inside Lovable.
2. Connect Lovable to GitHub.
3. Export or sync the project into this repository.
4. Move the project into the appropriate folder under `exports/`.
5. Add a short `NOTES.md` file for context.
6. Use Codex, Claude Code, or another development tool to inspect, refactor, extend, or productionise the code.
7. Move reusable elements into the `reusable/` folder.

---

## Naming Conventions

Use clear, lowercase folder names with hyphens or underscores.

Recommended:

```text
nilelor-reviewer-ui_2026-06-13
landing-page-v1_2026-06-13
auth-flow-test_2026-06-13
```

Avoid vague names like:

```text
test
new-app
final
final-final
copy
```

---

## What Not to Commit

Do not commit:

- API keys
- Access tokens
- `.env` files
- Passwords
- Private credentials
- Payment provider secrets
- Supabase service-role keys
- Firebase private keys
- Large dependency folders such as `node_modules/`
- Build output folders unless specifically needed

---

## Security Note

Before using any exported project in production, review:

- Authentication logic
- API routes
- Environment variable handling
- Database permissions
- Input validation
- Error handling
- User data handling
- Payment or subscription logic

Lovable-generated code should be reviewed before production use.

---

## Status

This repository is maintained as a personal/project export and reuse hub.
