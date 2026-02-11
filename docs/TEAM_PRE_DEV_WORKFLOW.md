# Team Pre-Development Workflow

## 1. Purpose
This document standardizes what the team must do before coding starts, so we reduce repeated communication, scope drift, and API mismatch.

## 2. Required Outputs Before Coding (Minimum Set)
For each new feature/module, prepare at least:

1. `ROLE_MVP_REQUIREMENTS.md` (what to build)
2. `DEVELOPMENT_GUIDE.md` (how to build)
3. `DATA_API_CONTRACT.md` (data and API alignment)
4. `SERVER_DEPLOY_QUICKSTART.md` (deployment path)
5. A task card for the current implementation (template below)

## 3. UI Prototype Requirements
Use low-fidelity design first, then formal implementation:

1. Put wireframes/sketches in `docs/wireframes/`
2. Put static HTML prototypes in `docs/prototypes/`
3. Only production-ready pages go into business code folders (for example `src/pages/`)
4. Prototypes may include lightweight interaction logic (routing, modal toggle, form validation with mock data, loading/empty/error/success states).
5. Prototypes must not include real business integration (no production DB, no real auth flow, no complex backend coupling).

## 4. Standard Execution Order
1. Confirm MVP scope boundaries first.
2. Confirm data models and API contracts next.
3. Confirm UI wireframe and page states (loading/empty/error/success).
4. Create a task card, then start coding.

## 5. Global 30% + Local 100% Execution Rule
1. Define a global baseline first (about 30%): MVP scope, module boundaries, tech stack, and deployment path.
2. Implement by increments (100% for each increment): one closed-loop feature at a time.
3. For each increment, follow this order: scope -> wireframe -> API contract -> coding -> test.
4. After each increment, update documents before starting the next one.

## 6. Pre-Dev Checklist
- [ ] Goal is clear in one sentence
- [ ] In Scope and Out of Scope are explicit
- [ ] Core user journey is documented
- [ ] API request/response is defined in `DATA_API_CONTRACT.md`
- [ ] Error codes and edge cases are defined
- [ ] UI wireframe or HTML prototype exists
- [ ] Acceptance criteria are testable
- [ ] Allowed file-change scope is explicit

## 7. Task Card Template (Mandatory)
```text
Task:
Goal:
In Scope:
Out of Scope:
Files Allowed to Change:
API/Contract References:
UI References:
Acceptance Criteria:
Non-Goals:
```

## 8. Standard Prompt for AI (Copy/Paste)
```text
Use these files as source of truth:
- ROLE_MVP_REQUIREMENTS.md
- DEVELOPMENT_GUIDE.md
- DATA_API_CONTRACT.md
- SERVER_DEPLOY_QUICKSTART.md
- docs/TEAM_PRE_DEV_WORKFLOW.md

Implement only this task:
Task:
Goal:
In Scope:
Out of Scope:
Files Allowed to Change:
API/Contract References:
UI References:
Acceptance Criteria:
```

## 9. Handoff Requirements
After finishing work, always provide:

1. Code change summary (which files changed and why)
2. Contract changes (if any)
3. Documentation updates (if any)
4. Test results and known risks

## 10. Change Log
| Date | Version | Change | Author |
|---|---|---|---|
| `2026-02-11` | `v0.1.1` | `Add Global 30% + Local 100% execution rule` | `Codex` |
| `2026-02-11` | `v0.1.0` | `Initial team workflow` | `Codex` |
