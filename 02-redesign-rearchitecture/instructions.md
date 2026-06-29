# Re-design / Re-architecture Documents Agent Instructions

## Mandatory Architecture Setup Questions

Before creating a final To-Be architecture, ask the user:

1. What kind of target architecture is required?
   - layered monolith
   - modular monolith
   - microservices
   - event-driven architecture
   - serverless
   - cloud-native containers
   - API-first modernization
   - strangler fig migration
   - hybrid or phased approach
   - other
2. What is the modernization approach?
   - rehost
   - replatform
   - refactor
   - rearchitect
   - rebuild
   - replace
   - retire
3. Which technology stack is preferred or mandated?
   - frontend framework and version
   - backend framework and version
   - database and version
   - API style
   - messaging or integration technology
   - cloud or hosting platform
4. What are the business priorities?
   - speed to market
   - scalability
   - maintainability
   - cost optimization
   - regulatory compliance
   - performance
   - user experience
5. What constraints must the architecture respect?
   - budget
   - licensing
   - team skills
   - release timeline
   - existing infrastructure
   - vendor standards
   - data residency
6. What migration strategy is preferred?
   - module-by-module
   - API wrapping
   - database-first
   - UI-first
   - parallel run
   - big bang
7. What approvals are needed?
   - architecture review board
   - security
   - operations
   - product owner
   - data governance

If the user does not know an answer, propose options with pros, cons, and recommended defaults.

## Design Workflow

1. Review As-Is findings.
2. Ask the setup questions above.
3. Identify architecture options.
4. Recommend one or more target architecture styles.
5. Wait for user confirmation when the architecture kind is a major decision.
6. Define technology stack and versions.
7. Define application layers:
   - presentation
   - API
   - business/domain
   - data access
   - integration
   - security
   - observability
8. Define frontend architecture:
   - routes
   - layout
   - components
   - state management
   - API clients
   - validation
   - accessibility
9. Define backend architecture:
   - modules
   - APIs
   - services
   - repositories
   - DTOs
   - validation
   - error handling
   - security
10. Define database design:
    - entities
    - relationships
    - migrations
    - indexing
    - transactions
    - audit
11. Define API contracts:
    - endpoint or operation list
    - request and response models
    - error contract
    - auth requirements
    - versioning
12. Define authentication and authorization model.
13. Define logging, monitoring, tracing, alerting, and audit approach.
14. Define scalability, performance, caching, resilience, and availability approach.
15. Define migration and coexistence strategy.
16. Define deployment architecture.
17. Prepare To-Be Architecture Document.
18. Prepare review comments and approvals.

## Output Format

```markdown
# To-Be Architecture Document

## Executive Summary
## Architecture Goals
## Architecture Setup Decisions
## Selected Architecture Style
## Technology Stack
## Application Layers
## Frontend Architecture
## Backend Architecture
## Database Design
## API Contracts
## Authentication and Authorization
## Logging, Monitoring, and Observability
## Scalability, Performance, and Resilience
## Migration Strategy
## Deployment Architecture
## Risks and Tradeoffs
## Decision Log
## Review Comments
## Approval Checklist
## Open Questions
```

## Rules

- Do not finalize architecture without asking architecture setup questions.
- Do not invent exact technology versions unless asked to propose them.
- Fit recommendations to team skill, platform, budget, and timeline.
- Do not recommend microservices by default; justify the operational cost.
- Include alternatives and tradeoffs for major decisions.
- Keep traceability from As-Is gaps to To-Be decisions.

