# Re-design / Re-architecture Documents Sub-Agents

These sub-agents execute the target architecture workflow step by step. The workflow must not finalize the To-Be Architecture Document until architecture setup questions are answered or assumptions are explicitly approved.

## Step-by-Step Sub-Agent Flow

| Step | Sub-Agent | Purpose | Primary Output |
|---|---|---|---|
| 1 | `architecture-intake-questionnaire-agent` | Ask what kind of new architecture is required, modernization approach, target stack, constraints, migration preference, and approvals. | Architecture intake answers |
| 2 | `as-is-context-reader-agent` | Read As-Is architecture, reverse engineering findings, gaps, risks, workflows, APIs, database, integrations, security, and deployment context. | Current-state context summary |
| 3 | `architecture-style-options-agent` | Propose suitable architecture styles such as layered, modular monolith, microservices, event-driven, serverless, strangler, or hybrid. | Architecture style options |
| 4 | `architecture-decision-agent` | Capture the user's selected architecture style or approved hybrid and record rationale. | Architecture decision record |
| 5 | `technology-stack-agent` | Define or validate frontend, backend, database, integration, hosting, identity, observability, and reporting technologies with versions. | Target technology stack |
| 6 | `application-layer-agent` | Define application layers, responsibilities, boundaries, dependency direction, and shared cross-cutting concerns. | Application layer model |
| 7 | `frontend-architecture-agent` | Define frontend routes, modules, layouts, components, state management, API clients, validation, accessibility, and build approach. | Frontend architecture |
| 8 | `backend-architecture-agent` | Define backend modules, APIs, services, repositories, DTOs, validation, security, errors, logging, and background processing. | Backend architecture |
| 9 | `database-design-agent` | Define target data model, ownership, migration strategy, indexing, transactions, audit, retention, and reporting data approach. | Database design |
| 10 | `api-contract-agent` | Define API endpoints or operations, request and response models, status codes, errors, auth requirements, and versioning. | API contract specification |
| 11 | `auth-authorization-agent` | Define identity provider, authentication, authorization, roles, policies, token/session flow, secrets, and compliance controls. | Auth and authorization model |
| 12 | `observability-scalability-agent` | Define logging, metrics, tracing, alerting, audit, performance, caching, resilience, scaling, and availability approach. | Observability and scalability design |
| 13 | `migration-strategy-agent` | Define migration waves, coexistence, data migration, cutover, rollback, dependency sequencing, and release strategy. | Migration strategy |
| 14 | `deployment-architecture-agent` | Define environments, runtime topology, infrastructure, containers, cloud/on-prem platform, network, config, and release path. | Deployment architecture |
| 15 | `to-be-document-writer-agent` | Prepare the To-Be Architecture Document and supporting architecture docs. | To-Be documentation package |
| 16 | `review-approval-agent` | Prepare review comments, approval checklist, decision log, risks, assumptions, and open items. | Review and approval package |

## Mandatory Question Gate

The `architecture-intake-questionnaire-agent` must ask:

- What kind of target architecture is required?
- Which modernization approach is expected?
- What target stack and versions should be used?
- What constraints, NFRs, compliance needs, team skills, and timelines apply?
- What migration strategy is preferred?
- Which review and approval gates are required?

## Required Final Package

```text
docs/architecture/
|-- README.md
|-- 01-TO-BE-ARCHITECTURE.md
|-- 02-TARGET-TECH-STACK.md
|-- 03-APPLICATION-LAYERS.md
|-- 04-FRONTEND-ARCHITECTURE.md
|-- 05-BACKEND-ARCHITECTURE.md
|-- 06-DATABASE-DESIGN.md
|-- 07-API-CONTRACTS.md
|-- 08-SECURITY-AUTHORIZATION.md
|-- 09-OBSERVABILITY-SCALABILITY.md
|-- 10-MIGRATION-DEPLOYMENT-STRATEGY.md
|-- 11-DECISION-LOG.md
|-- 12-REVIEW-COMMENTS-APPROVALS.md
```

