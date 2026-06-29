# Reverse Engineering Documents Sub-Agents

These sub-agents execute the Reverse Engineering Documents Agent workflow step by step. The main agent should route through them in order, skipping only steps that are explicitly out of scope or already completed with evidence.

## Step-by-Step Sub-Agent Flow

| Step | Sub-Agent | Purpose | Primary Output |
|---|---|---|---|
| 1 | `document-intake-agent` | Collect existing documents, README files, architecture notes, API specs, database docs, deployment guides, and test plans. | Source document inventory |
| 2 | `codebase-analysis-agent` | Analyze current source structure, languages, frameworks, build tools, dependencies, configuration, and entry points. | Codebase analysis summary |
| 3 | `module-identification-agent` | Identify application modules, packages, features, domains, shared libraries, generated code, and ownership boundaries. | Module inventory |
| 4 | `business-workflow-agent` | Understand actors, roles, workflows, business rules, approvals, exception paths, and operational journeys. | Business workflow map |
| 5 | `frontend-screen-navigation-agent` | Identify frontend routes, screens, forms, navigation paths, UI components, client state, and API usage. | Screen and navigation catalog |
| 6 | `backend-api-service-agent` | Identify controllers, routes, handlers, APIs, services, DTOs, validation, errors, and service dependencies. | Backend API and service catalog |
| 7 | `database-schema-agent` | Analyze tables, views, collections, relationships, constraints, indexes, migrations, stored logic, and data ownership. | Database schema documentation |
| 8 | `integration-analysis-agent` | Identify third-party systems, API calls, queues, files, events, protocols, retries, and failure handling. | Integration inventory |
| 9 | `batch-scheduled-task-agent` | Identify cron jobs, schedulers, background workers, ETL jobs, reports, and operational scripts. | Batch and scheduled task catalog |
| 10 | `security-authentication-agent` | Capture identity provider, login/logout, sessions, tokens, roles, permissions, policies, secrets, and certificates. | Security and auth flow |
| 11 | `deployment-process-agent` | Capture build, packaging, environment configuration, infrastructure, deployment scripts, release process, and rollback evidence. | Deployment process summary |
| 12 | `as-is-architecture-writer-agent` | Prepare the As-Is Architecture Document using evidence from prior sub-agents. | As-Is Architecture Document |
| 13 | `gap-risk-opportunity-agent` | Prepare gaps, risks, constraints, technical debt, modernization opportunities, and open questions. | Gap, risk, and modernization opportunity report |

## Handoff Rules

- Each sub-agent must list evidence sources and open questions.
- Facts, inferences, and assumptions must be separated.
- Later sub-agents must reuse earlier outputs instead of re-scanning unnecessarily.
- The final writer must include traceability from source evidence to architecture statements.

## Required Final Package

```text
docs/reverse-engineering/
|-- README.md
|-- 01-AS-IS-ARCHITECTURE.md
|-- 02-MODULE-INVENTORY.md
|-- 03-BUSINESS-WORKFLOWS.md
|-- 04-FRONTEND-SCREENS-NAVIGATION.md
|-- 05-BACKEND-APIS-SERVICES.md
|-- 06-DATABASE-SCHEMA.md
|-- 07-INTEGRATIONS-BATCH-SECURITY.md
|-- 08-DEPLOYMENT-PROCESS.md
|-- 09-GAPS-RISKS-OPPORTUNITIES.md
```

