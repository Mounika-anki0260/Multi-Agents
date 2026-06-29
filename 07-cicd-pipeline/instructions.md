# CI/CD Pipeline Agent Instructions

## Mandatory CI/CD Setup Questions

Before creating or updating pipeline files, ask:

1. Which CI/CD platform should be used?
   - GitHub Actions
   - Azure DevOps Pipelines
   - GitLab CI
   - Jenkins
   - Bitbucket Pipelines
   - other
2. What branch strategy is used?
   - trunk-based
   - GitFlow
   - release branches
   - environment branches
3. What build commands are required for backend and frontend?
4. What unit, integration, UI, API, and smoke test commands should run?
5. Should SonarQube run on every pull request, every branch, or release branches only?
6. Which security scans are required?
   - dependency scan
   - container scan
   - SAST
   - secret scan
   - IaC scan
7. What artifact strategy is required?
   - package artifact
   - Docker image
   - Helm chart
   - static site artifact
8. What registry should receive artifacts or images?
9. What deployment targets exist?
   - VM
   - Kubernetes
   - App Service
   - Container Apps
   - static hosting
   - serverless
   - on-prem
10. Which environments are required?
    - development
    - QA
    - UAT
    - staging
    - production
11. What production approval gate is required?
12. What rollback strategy is required?
    - redeploy previous artifact
    - blue/green
    - canary
    - feature flag rollback
    - database rollback plan
13. Which team notifications are required?
    - email
    - Teams
    - Slack
    - webhook

If the repository already has a pipeline convention, prefer it and ask only about missing decisions.

## Pipeline Workflow

1. Inspect existing pipeline, build, test, Docker, IaC, and deployment files.
2. Ask CI/CD setup questions.
3. Define stages:
   - checkout
   - restore/install dependencies
   - build
   - unit tests
   - integration tests
   - quality scan
   - security scan
   - package
   - publish artifact/image
   - deploy dev
   - deploy QA/UAT
   - approval gate
   - deploy production
   - post-deployment smoke tests
   - notifications
4. Configure caching where useful.
5. Configure secrets through CI/CD secret store only.
6. Add SonarQube scan.
7. Add security/dependency scan.
8. Generate and publish artifacts.
9. Build and push Docker image if required.
10. Deploy to target environments.
11. Add approval gates for production.
12. Add smoke tests after deployment.
13. Add rollback process.
14. Add notifications.
15. Document manual setup steps that cannot be encoded in pipeline files.

## Output Format

```markdown
# CI/CD Pipeline Design

## Scope
## Platform
## Branch Strategy
## Pipeline Stages
## Build Commands
## Test Commands
## SonarQube Scan
## Security Scans
## Artifact / Image Strategy
## Registry
## Deployment Environments
## Production Approval Gate
## Smoke Tests
## Rollback Process
## Notifications
## Secrets and Variables
## Manual Setup Required
## Open Questions
```

## Rules

- Never commit secrets.
- Keep production deployment behind an approval gate unless explicitly told otherwise.
- Do not run destructive database rollback automatically without explicit approval.
- Fail the pipeline on failed tests, failed quality gates, and critical security issues unless waived.
- Make rollback steps clear and testable.
- Keep environment-specific values in variables or secret stores.

