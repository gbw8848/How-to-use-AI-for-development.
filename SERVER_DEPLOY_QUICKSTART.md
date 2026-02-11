# SERVER_DEPLOY_QUICKSTART

## 1. Document Control
- Project: `TODO_PROJECT_NAME`
- Version: `v0.1.0`
- Owner: `TODO_OWNER`
- Last Updated: `YYYY-MM-DD`
- Status: `Draft | Active | Archived`

## 2. Deployment Targets
| Environment | URL | Infra | Branch | Auto Deploy |
|---|---|---|---|---|
| `dev` | `TODO` | `TODO` | `develop` | `Yes/No` |
| `staging` | `TODO` | `TODO` | `staging` | `Yes/No` |
| `prod` | `TODO` | `TODO` | `main` | `Yes/No` |

## 3. Prerequisites
- Access:
  - [ ] Repository access
  - [ ] Server/Cloud access
  - [ ] Secret manager access
- Local tools:
  - [ ] `git`
  - [ ] `docker` / `docker compose` (if used)
  - [ ] Runtime (`node/python/go/etc`) version: `TODO`
- Required files:
  - [ ] `.env`
  - [ ] Deployment config (`TODO`)

## 4. Environment Variables
| Name | Required | Example | Description | Source |
|---|---|---|---|---|
| `APP_ENV` | `Yes` | `production` | `Runtime env` | `TODO` |
| `PORT` | `Yes` | `8080` | `Service port` | `TODO` |
| `DATABASE_URL` | `Yes` | `postgres://...` | `DB connection` | `TODO` |
| `JWT_SECRET` | `Yes` | `***` | `Auth signing key` | `Secret Manager` |
| `TODO_VAR` | `Yes/No` | `TODO` | `TODO` | `TODO` |

## 5. Build and Release
### Option A: Docker Compose
```bash
# 1) Pull latest code
git fetch --all
git checkout main
git pull --rebase

# 2) Build and run
docker compose pull
docker compose build --no-cache
docker compose up -d

# 3) Verify
docker compose ps
```

### Option B: Process Manager (Example)
```bash
# 1) Pull latest code
git fetch --all
git checkout main
git pull --rebase

# 2) Install and build
TODO_INSTALL_COMMAND
TODO_BUILD_COMMAND

# 3) Restart service
TODO_RESTART_COMMAND
```

## 6. Database Migration
- Migration command: `TODO_MIGRATE_COMMAND`
- Seed command (optional): `TODO_SEED_COMMAND`
- Rollback migration command: `TODO_MIGRATE_ROLLBACK_COMMAND`

## 7. Post-Deploy Verification
- [ ] Service health endpoint returns 200: `GET /health`
- [ ] Core API smoke test passed: `TODO_ENDPOINT`
- [ ] Web/app loads correctly
- [ ] Error logs show no new critical issues
- [ ] Metrics within expected baseline

## 8. Rollback Procedure
1. Identify last known good release/tag: `TODO_TAG`.
2. Re-deploy previous release:
```bash
git checkout TODO_PREVIOUS_TAG
TODO_DEPLOY_COMMAND
```
3. Run smoke test and confirm recovery.
4. Record incident and root cause.

## 9. Monitoring and Alerts
- Logs: `TODO_LOG_PLATFORM`
- Metrics: `TODO_METRICS_PLATFORM`
- Error tracking: `TODO_ERROR_TRACKING`
- Alert channels: `TODO_SLACK_EMAIL_PAGER`
- On-call owner: `TODO_OWNER`

## 10. Common Failure Cases
| Symptom | Likely Cause | Quick Check | Fix |
|---|---|---|---|
| `Service not starting` | `Missing env vars` | `printenv` | `Set required vars` |
| `DB connection error` | `Network/credentials` | `test connection` | `Fix SG/VPC/creds` |
| `502/504` | `Upstream unhealthy` | `health checks` | `Restart upstream` |

## 11. Release Checklist
- [ ] Code merged and tagged
- [ ] Migrations reviewed
- [ ] Secrets configured
- [ ] Deployment executed
- [ ] Verification completed
- [ ] Rollback plan validated

## 12. Change Log
| Date | Version | Change | Author |
|---|---|---|---|
| `YYYY-MM-DD` | `v0.1.0` | `Initial template` | `Codex` |

