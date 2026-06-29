# SonarQube / Code Quality Agent Instructions

## Mandatory Code Quality Setup Questions

Before configuring scans or quality gates, ask:

1. Are we using SonarQube Server or SonarCloud?
2. What is the project key, organization, and project name?
3. What languages and frameworks are in scope?
4. Which scanner should be used?
   - SonarScanner CLI
   - Maven plugin
   - Gradle plugin
   - .NET scanner
   - npm-based scanner
   - CI task/action
5. What quality gate thresholds are required?
   - coverage
   - duplicated lines
   - reliability rating
   - security rating
   - maintainability rating
   - blocker/critical issue count
6. What coverage reports are produced and where are they located?
7. Which branches and pull request events should trigger scans?
8. Who owns issue assignment and remediation?
9. Should blocker and critical issues fail the pipeline?
10. Are any files, generated folders, migrations, or test fixtures excluded?

If the repository already has SonarQube configuration, prefer it and ask only about missing decisions.

## Workflow

1. Inspect repository language, build, test, and coverage setup.
2. Ask code quality setup questions.
3. Create or update SonarQube project configuration.
4. Configure scanner command or CI task.
5. Configure quality gate thresholds.
6. Configure coverage report paths.
7. Enable code smell, vulnerability, security hotspot, and duplicate code checks.
8. Integrate scan into CI/CD and pull request validation.
9. Run or document the scan command.
10. Generate quality report.
11. Categorize issues:
    - blocker
    - critical
    - major
    - minor
    - info
12. Assign issues to owners.
13. Fix blocker and critical issues first.
14. Re-run scan.
15. Approve only after quality gate passes or accepted waivers are documented.

## Output Format

```markdown
# Code Quality Report

## Scope
## SonarQube Project Setup
## Scanner Configuration
## Quality Gate
## Coverage Threshold
## Code Smell Checks
## Vulnerability Checks
## Duplicate Code Checks
## CI/CD Integration
## Pull Request Scan Policy
## Scan Results
## Issues By Severity
## Remediation Plan
## Re-Scan Result
## Approval Status
## Open Questions
```

## Rules

- Never commit tokens or secrets.
- Do not lower thresholds without explicit user approval.
- Prefer fixing issues over suppressing them.
- Suppress only false positives and document the reason.
- Treat blocker and critical vulnerabilities as release blockers unless explicitly waived.
- Keep generated code exclusions specific and justified.

