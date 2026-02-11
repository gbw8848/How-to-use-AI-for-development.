# DEVELOPMENT_GUIDE

## 1. Document Control
- Project: `TODO_PROJECT_NAME`
- Version: `v0.1.0`
- Owner: `TODO_OWNER`
- Last Updated: `YYYY-MM-DD`
- Status: `Draft | Active | Archived`

## 2. Purpose and Priority
- Purpose: Define engineering rules so all changes stay consistent.
- Rule priority:
1. `ROLE_MVP_REQUIREMENTS.md` (what to build)
2. `DATA_API_CONTRACT.md` (data/interface contract)
3. `DEVELOPMENT_GUIDE.md` (implementation standards)
4. Task-specific requirements

## 3. Tech Stack
- Frontend: `TODO`
- Backend: `TODO`
- Database: `TODO`
- Cache/Queue: `TODO`
- Infra/Cloud: `TODO`
- Package Manager: `TODO`

## 4. Architecture Rules
- Pattern: `Monolith | Modular Monolith | Microservices | Other`
- Service boundaries: `TODO`
- Module ownership: `TODO`
- Cross-module dependency rules: `TODO`

## 5. Directory and Naming Conventions
- Source layout:
  - `TODO_PATH_1`
  - `TODO_PATH_2`
  - `TODO_PATH_3`
- File naming: `kebab-case | snake_case | PascalCase`
- Symbol naming:
  - Variables/functions: `camelCase | snake_case`
  - Types/classes: `PascalCase`
  - Constants: `UPPER_SNAKE_CASE`

## 6. Coding Standards
- Language version: `TODO`
- Lint/format tools: `TODO`
- Max function complexity guideline: `TODO`
- Comment policy: Explain intent, not obvious syntax.
- Forbidden patterns:
  - `TODO_ANTI_PATTERN_1`
  - `TODO_ANTI_PATTERN_2`

## 7. API and State Handling
- API client pattern: `TODO`
- Error envelope handling: `TODO`
- Retry/timeout policy: `TODO`
- State management approach: `TODO`
- Caching strategy: `TODO`

## 8. Error Handling and Logging
- User-facing errors: `TODO_STYLE`
- Internal error codes: `TODO_FORMAT`
- Logging levels: `DEBUG/INFO/WARN/ERROR`
- Sensitive data redaction rules: `TODO`
- Correlation/request ID policy: `TODO`

## 9. Security Baseline
- Auth method: `TODO`
- Authz strategy (RBAC/ABAC): `TODO`
- Secrets management: `TODO`
- Input validation standard: `TODO`
- Dependency scanning policy: `TODO`

## 10. Testing Strategy
- Unit tests: `Required | Optional`
- Integration tests: `Required | Optional`
- E2E tests: `Required | Optional`
- Minimum coverage target: `TODO%`
- Test data policy: `TODO`

## 11. CI/CD Expectations
- CI pipeline checks:
  - [ ] Lint
  - [ ] Type check
  - [ ] Tests
  - [ ] Build
- Merge policy: `TODO`
- Release tagging format: `vMAJOR.MINOR.PATCH`

## 12. Definition of Done
A task is done only if:
- [ ] Scope matches `ROLE_MVP_REQUIREMENTS.md`
- [ ] Contract matches `DATA_API_CONTRACT.md`
- [ ] Tests pass
- [ ] Logs/errors follow this guide
- [ ] Docs updated where needed

## 13. Task Template (For AI or Human)
Use this structure for every implementation request:

```text
Task:
Goal:
In Scope:
Out of Scope:
Files Allowed to Change:
Acceptance Criteria:
Contract References:
Notes:
```

## 14. Change Log
| Date | Version | Change | Author |
|---|---|---|---|
| `YYYY-MM-DD` | `v0.1.0` | `Initial template` | `Codex` |
