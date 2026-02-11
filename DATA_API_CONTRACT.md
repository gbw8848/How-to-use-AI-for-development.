# DATA_API_CONTRACT

## 1. Document Control
- Project: `TODO_PROJECT_NAME`
- Version: `v0.1.0`
- Owner: `TODO_OWNER`
- Last Updated: `YYYY-MM-DD`
- Status: `Draft | Active | Archived`

## 2. Contract Principles
- Naming style: `TODO` (example: `snake_case` for DB, `camelCase` for API JSON)
- Time format: `ISO-8601 UTC`
- ID format: `UUID | Snowflake | Auto Increment`
- Null handling: `TODO_RULE`
- Pagination style: `page/pageSize | cursor`
- Backward compatibility rule: `No breaking changes without version bump`

## 3. Standard API Envelope
### Success
```json
{
  "success": true,
  "data": {},
  "meta": {
    "requestId": "TODO",
    "timestamp": "2026-01-01T00:00:00Z"
  }
}
```

### Error
```json
{
  "success": false,
  "error": {
    "code": "TODO_CODE",
    "message": "TODO_MESSAGE",
    "details": []
  },
  "meta": {
    "requestId": "TODO",
    "timestamp": "2026-01-01T00:00:00Z"
  }
}
```

## 4. Domain Models
| Model | Description | Primary Key | Key Fields |
|---|---|---|---|
| `TODO_MODEL_1` | `TODO` | `TODO` | `TODO` |
| `TODO_MODEL_2` | `TODO` | `TODO` | `TODO` |

## 5. Database Schema (Template)
### Table: `TODO_TABLE_NAME`
| Column | Type | Nullable | Default | Constraints | Description |
|---|---|---|---|---|---|
| `id` | `TODO` | `No` | `TODO` | `PK` | `Primary ID` |
| `created_at` | `timestamp` | `No` | `now()` |  | `Creation time` |
| `updated_at` | `timestamp` | `No` | `now()` |  | `Update time` |
| `TODO_COLUMN` | `TODO` | `Yes/No` | `TODO` | `TODO` | `TODO` |

Indexes:
- `TODO_INDEX_1`
- `TODO_INDEX_2`

## 6. API Endpoint Catalog
| Endpoint | Method | Auth | Request | Response | Notes |
|---|---|---|---|---|---|
| `/api/TODO_RESOURCE` | `GET` | `Yes/No` | `Query params` | `List/Item` | `TODO` |
| `/api/TODO_RESOURCE` | `POST` | `Yes/No` | `JSON body` | `Created item` | `TODO` |

## 7. Endpoint Detail Template
### `POST /api/TODO_RESOURCE`
Purpose: `TODO`

Request Body:
```json
{
  "TODO_FIELD": "TODO_VALUE"
}
```

Validation Rules:
- `TODO_FIELD`: `required`, `type`, `range/length`

Success Response (`201`):
```json
{
  "success": true,
  "data": {
    "id": "TODO_ID"
  },
  "meta": {
    "requestId": "TODO",
    "timestamp": "2026-01-01T00:00:00Z"
  }
}
```

Error Responses:
- `400` `TODO_BAD_REQUEST_CASE`
- `401` `TODO_UNAUTHORIZED_CASE`
- `409` `TODO_CONFLICT_CASE`
- `500` `TODO_INTERNAL_CASE`

## 8. State and Event Contracts (Optional)
- Event name: `TODO_EVENT`
- Producer: `TODO`
- Consumer: `TODO`
- Payload schema: `TODO`
- Retry/dead-letter policy: `TODO`

## 9. Contract Test Checklist
- [ ] Request validation tests exist
- [ ] Response schema tests exist
- [ ] Error code mapping tests exist
- [ ] Backward compatibility tests exist

## 10. Change Log
| Date | Version | Change | Author |
|---|---|---|---|
| `YYYY-MM-DD` | `v0.1.0` | `Initial template` | `Codex` |

