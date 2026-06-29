# CI/CD Pipeline Sub-Agents

These sub-agents execute delivery automation step by step. The main CI/CD Pipeline Agent must ask platform, branch, environment, deployment, approval, rollback, and notification questions before creating or changing pipeline files.

## Step-by-Step Sub-Agent Flow

| Step | Sub-Agent | Purpose | Primary Output |
|---|---|---|---|
| 1 | `cicd-setup-questionnaire-agent` | Ask CI/CD platform, branch strategy, build/test commands, scans, artifact strategy, registry, environments, approvals, rollback, and notifications. | CI/CD setup decisions |
| 2 | `pipeline-stage-agent` | Define stages, dependencies, conditions, parallel jobs, environment promotions, and failure behavior. | Pipeline stage design |
| 3 | `source-checkout-agent` | Configure repository checkout, branch filters, pull request triggers, tags, submodules, and permissions. | Source checkout setup |
| 4 | `dependency-install-agent` | Install backend, frontend, infrastructure, test, and scanner dependencies with caching where appropriate. | Dependency install step |
| 5 | `build-agent` | Run backend, frontend, library, container, or static build commands. | Build step |
| 6 | `unit-test-agent` | Run unit tests and publish results and coverage. | Unit test step |
| 7 | `integration-test-agent` | Run integration tests, service containers, database setup, API checks, and publish results. | Integration test step |
| 8 | `sonarqube-scan-agent` | Run SonarQube scan, publish quality gate status, and fail pipeline when required. | SonarQube scan step |
| 9 | `security-dependency-scan-agent` | Run dependency, secret, SAST, container, and IaC scans as required. | Security scan step |
| 10 | `artifact-generation-agent` | Package build outputs, version artifacts, attach metadata, and publish artifacts. | Build artifact |
| 11 | `docker-image-agent` | Build Docker images, tag with version/commit, scan image, and prepare for registry push when required. | Docker image |
| 12 | `registry-push-agent` | Push packages, artifacts, Docker images, or Helm charts to the configured registry. | Published artifact/image |
| 13 | `dev-deployment-agent` | Deploy to development environment and capture deployment status. | Development deployment |
| 14 | `qa-uat-deployment-agent` | Deploy to QA/UAT/staging environments and coordinate test readiness. | QA/UAT deployment |
| 15 | `production-approval-agent` | Add production approval gate with required reviewers, checks, and risk acceptance. | Production approval gate |
| 16 | `production-deployment-agent` | Deploy to production using the approved strategy and record version, environment, and deployment status. | Production deployment |
| 17 | `post-deployment-smoke-agent` | Run smoke tests after deployment and fail or alert on critical failures. | Smoke test result |
| 18 | `rollback-agent` | Define rollback process using previous artifact, blue/green, canary, feature flag, or manual rollback steps. | Rollback plan |
| 19 | `notification-agent` | Notify team on success, failure, approval waiting, rollback, and release completion. | Notification setup |

## Mandatory CI/CD Question Gate

The `cicd-setup-questionnaire-agent` must ask:

- Which CI/CD platform and branch strategy should be used?
- What build and test commands are required?
- What SonarQube and security scans should run?
- What artifact or Docker image strategy is required?
- What environments and deployment targets exist?
- What production approval, rollback, and notification process is required?

## Handoff Rules

- Secrets must stay in CI/CD secret stores.
- Production deployment should have an approval gate unless explicitly waived.
- Failed tests, failed quality gates, and critical security issues should block promotion unless waived.
- Destructive rollback or database rollback must require explicit approval.

