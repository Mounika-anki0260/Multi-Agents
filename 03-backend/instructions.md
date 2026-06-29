# Backend Agent Instructions

## Mandatory Backend Setup Questions

Before creating backend layers or scaffolding a new backend project, ask:

1. What backend technology and version should be used?
   - Java Spring Boot
   - .NET
   - Node.js / Express / NestJS
   - Python FastAPI / Django
   - Go
   - other
2. How should the project structure look?
   - package by layer
   - package by feature/domain
   - clean architecture
   - hexagonal architecture
   - modular monolith
   - microservice per bounded context
   - existing repository pattern
3. What layers are expected?
   - controller/resource
   - DTO/request/response
   - service/application
   - domain/model
   - repository/data access
   - mapper
   - validator
   - security
   - exception handling
   - configuration
4. What database and access pattern should be used?
   - ORM
   - SQL mapper
   - direct SQL
   - stored procedure integration
   - NoSQL client
5. What API style is required?
   - REST
   - GraphQL
   - gRPC
   - messaging/event-driven
   - batch/file-based
6. What authentication and authorization model is required?
   - JWT
   - OAuth2/OIDC
   - session-based
   - API key
   - mTLS
   - RBAC/ABAC
7. What validation, exception, and logging standards should be followed?
8. What test framework and coverage threshold should be used?
9. Should the agent create a new project, extend an existing project, or only prepare design/docs?

If the repository already has a backend convention, prefer it and ask only about missing decisions.

## Implementation Workflow

1. Read backend architecture, API contracts, and existing code.
2. Confirm backend setup answers.
3. Create or update project structure.
4. Configure environment profiles:
   - local
   - dev
   - QA/UAT
   - production
5. Configure database connection and migrations.
6. Implement entities/models.
7. Implement repositories/data access.
8. Implement services/business logic.
9. Implement controllers/API endpoints.
10. Implement DTOs and mapping.
11. Add validation.
12. Add authentication and authorization.
13. Add global exception handling.
14. Add structured logging and correlation IDs where applicable.
15. Add unit tests.
16. Add integration tests.
17. Run build and tests.
18. Run lint/static analysis/SonarQube if available.
19. Fix blocker, critical, and high-priority issues.
20. Prepare PR summary, test evidence, and review notes.

## Output Format For Backend Notes

```markdown
# Backend Implementation Notes

## Scope
## Project Structure
## Environment Profiles
## Database Connection
## Entities and Models
## Repositories
## Services
## Controllers and APIs
## DTOs and Validation
## Authentication and Authorization
## Exception Handling
## Logging
## Tests Added
## Quality Checks
## SonarQube Issues Fixed
## Pull Request Checklist
## Open Questions
```

## Rules

- Prefer existing project conventions.
- Keep business logic out of controllers.
- Keep persistence details out of API contracts.
- Validate all external inputs.
- Do not hardcode secrets.
- Add tests for success, validation failure, auth failure, and error paths.
- Document any skipped tests or quality checks.

