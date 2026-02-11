# How to use AI for development

This repository provides a practical documentation system for AI-assisted software development.

## Core documents

- `ROLE_MVP_REQUIREMENTS.md`: Defines product scope and MVP boundaries (what to build).
- `DEVELOPMENT_GUIDE.md`: Defines engineering rules and coding standards (how to build).
- `DATA_API_CONTRACT.md`: Defines data models and API contracts (how systems agree).
- `SERVER_DEPLOY_QUICKSTART.md`: Defines deployment and rollback flow (how to ship safely).

## Recommended workflow

1. Fill `ROLE_MVP_REQUIREMENTS.md` first.
2. Fill `DATA_API_CONTRACT.md` for key entities and endpoints.
3. Fill `DEVELOPMENT_GUIDE.md` with stack, structure, and quality gates.
4. Fill `SERVER_DEPLOY_QUICKSTART.md` with environment and release steps.
5. For each implementation request, create a clear task with:
   - Goal
   - In scope
   - Out of scope
   - Files allowed to change
   - Acceptance criteria
6. Ask AI to implement only that task while following the 4 documents.
7. Update documents when requirements or contracts change.

## Task prompt template

```text
Use the project documents as source of truth:
- ROLE_MVP_REQUIREMENTS.md
- DEVELOPMENT_GUIDE.md
- DATA_API_CONTRACT.md
- SERVER_DEPLOY_QUICKSTART.md

Task:
Goal:
In Scope:
Out of Scope:
Files Allowed to Change:
Acceptance Criteria:
```

## Why this works

- Reduces context loss across chat sessions.
- Prevents scope creep and style drift.
- Improves API alignment between frontend and backend.
- Makes deployment repeatable.

## Repo structure

- `README.md`
- `ROLE_MVP_REQUIREMENTS.md`
- `DEVELOPMENT_GUIDE.md`
- `DATA_API_CONTRACT.md`
- `SERVER_DEPLOY_QUICKSTART.md`
