# Backend Sub-Agents

These sub-agents execute backend delivery step by step. The main Backend Agent must ask project structure questions before scaffolding or changing backend layers.

## Step-by-Step Sub-Agent Flow

| Step | Sub-Agent | Purpose | Primary Output |
|---|---|---|---|
| 1 | `backend-setup-questionnaire-agent` | Ask backend stack, version, project structure, layers, API style, database pattern, auth model, testing framework, and whether to create or extend a project. | Backend setup decisions |
| 2 | `backend-project-setup-agent` | Create or validate backend project setup, dependencies, build tool, runtime configuration, and developer commands. | Backend project baseline |
| 3 | `folder-package-structure-agent` | Define package/folder structure by feature, layer, clean architecture, hexagonal architecture, modular monolith, microservice, or existing pattern. | Backend structure map |
| 4 | `environment-profile-agent` | Configure local, dev, QA/UAT, staging, and production profiles using environment-safe configuration. | Environment profile setup |
| 5 | `database-connection-agent` | Set up database connection, pooling, migrations, ORM/SQL mapper/direct SQL, and local database configuration. | Database connectivity |
| 6 | `entity-model-agent` | Create entities, domain models, persistence models, enums, value objects, and relationships. | Entity/model layer |
| 7 | `repository-data-access-agent` | Create repositories, DAO classes, query objects, stored procedure adapters, or NoSQL data access components. | Data access layer |
| 8 | `service-business-logic-agent` | Implement services, use cases, transactions, business rules, orchestration, and domain logic. | Service/business layer |
| 9 | `controller-api-endpoint-agent` | Implement controllers, resources, route handlers, endpoints, status codes, and endpoint security declarations. | API endpoint layer |
| 10 | `request-response-dto-agent` | Add request DTOs, response DTOs, mappers, serialization rules, pagination, filtering, and sorting models. | DTO and mapping layer |
| 11 | `validation-agent` | Add input validation, business validation, constraint messages, and validation tests. | Validation layer |
| 12 | `authentication-authorization-agent` | Add authentication, authorization, role/policy checks, token/session handling, and secured endpoint tests. | Backend security implementation |
| 13 | `exception-handling-agent` | Add global exception handling, error contracts, domain exceptions, validation errors, and audit-safe error messages. | Error handling layer |
| 14 | `logging-agent` | Add structured logging, correlation IDs, request tracing, audit logs, and sensitive-data masking. | Logging implementation |
| 15 | `unit-test-agent` | Add unit tests for services, validators, mappers, error handling, and permission-sensitive logic. | Unit test coverage |
| 16 | `integration-test-agent` | Add integration tests for APIs, database access, transactions, external adapters, and auth behavior. | Integration test coverage |
| 17 | `code-quality-agent` | Run build, tests, linting, formatting, static analysis, and coverage checks. | Code quality result |
| 18 | `sonarqube-fix-agent` | Fix SonarQube blocker, critical, vulnerability, duplication, and code smell issues. | SonarQube remediation |
| 19 | `pull-request-agent` | Prepare PR summary, changed files, tests run, risk notes, screenshots/logs where useful, and review checklist. | Pull request readiness |
| 20 | `code-review-merge-agent` | Support review comments, update code, rerun checks, and confirm merge readiness. | Merge readiness status |

## Mandatory Backend Question Gate

The `backend-setup-questionnaire-agent` must ask:

- What backend stack and version should be used?
- How should the project structure look?
- Which layers and package conventions are expected?
- Which database and data access approach should be used?
- Which API, auth, validation, logging, and testing standards apply?
- Should this create a new project, extend an existing project, or only document the backend design?

## Handoff Rules

- Project setup decisions must be recorded before code generation.
- API contracts and database design must be referenced by implementation sub-agents.
- Tests and quality checks are required before PR readiness.
- Secrets must stay outside source control.

