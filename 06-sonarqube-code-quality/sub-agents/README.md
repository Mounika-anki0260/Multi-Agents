# SonarQube / Code Quality Sub-Agents

These sub-agents execute code quality governance step by step. The main SonarQube / Code Quality Agent must ask quality gate questions before changing thresholds or scan configuration.

## Step-by-Step Sub-Agent Flow

| Step | Sub-Agent | Purpose | Primary Output |
|---|---|---|---|
| 1 | `quality-setup-questionnaire-agent` | Ask SonarQube/SonarCloud choice, project key, organization, languages, scanner, thresholds, coverage reports, branches, ownership, and exclusions. | Quality setup decisions |
| 2 | `sonarqube-project-setup-agent` | Set up or validate SonarQube project, project key, name, organization, permissions, and branch strategy. | SonarQube project setup |
| 3 | `scanner-configuration-agent` | Configure scanner CLI, Maven, Gradle, .NET, npm scanner, or CI task/action based on repository stack. | Scanner configuration |
| 4 | `quality-gate-agent` | Configure quality gate conditions for reliability, security, maintainability, coverage, duplication, and new-code policy. | Quality gate definition |
| 5 | `coverage-threshold-agent` | Define coverage thresholds and connect unit, integration, frontend, and backend coverage report paths. | Coverage configuration |
| 6 | `code-smell-agent` | Enable and review maintainability, complexity, naming, dead code, and code smell rules. | Code smell policy |
| 7 | `vulnerability-agent` | Enable and review vulnerability, security hotspot, dependency, injection, auth, crypto, and secret-related checks. | Security scan policy |
| 8 | `duplication-agent` | Enable duplicate code checks and define exclusions for generated code where justified. | Duplication policy |
| 9 | `cicd-integration-agent` | Integrate scans into CI/CD build, pull request validation, branch analysis, and release gates. | CI/CD quality integration |
| 10 | `pull-request-scan-agent` | Run or define pull request scan behavior, decoration, branch comparison, and failure conditions. | Pull request scan setup |
| 11 | `quality-report-agent` | Generate quality report with gate status, coverage, duplications, ratings, issues, and trends. | Quality report |
| 12 | `issue-assignment-agent` | Assign issues to owners by module, severity, category, or responsible team. | Issue assignment plan |
| 13 | `blocker-critical-fix-agent` | Fix or guide remediation for blocker and critical issues first. | Critical remediation |
| 14 | `rescan-agent` | Re-run scan after remediation and compare quality gate results. | Re-scan result |
| 15 | `quality-approval-agent` | Approve only after quality gate passes or documented waivers are accepted. | Quality approval status |

## Mandatory Code Quality Question Gate

The `quality-setup-questionnaire-agent` must ask:

- Are we using SonarQube Server or SonarCloud?
- What project key, organization, languages, scanner, and CI/CD platform are used?
- What coverage, duplication, reliability, security, and maintainability thresholds are required?
- Where are coverage reports generated?
- Which branches and pull request events should run scans?
- Who owns issue assignment and remediation?

## Handoff Rules

- Do not lower quality thresholds without explicit approval.
- Tokens and credentials must never be committed.
- Generated-code exclusions must be specific and justified.
- Blocker and critical issues remain release blockers unless waived.

