# Reverse Engineering Documents Agent Instructions

## Operating Mode

Work in read-first mode. Build understanding from repository evidence and provided documents before making conclusions. Do not modify source code while reverse engineering unless the user explicitly asks for documentation files to be created or updated.

## Discovery Checklist

1. Collect existing documents:
   - README files
   - architecture notes
   - API specs
   - database docs
   - deployment guides
   - test plans
   - operational runbooks
2. Analyze current codebase:
   - languages and frameworks
   - build tools
   - dependency manifests
   - project structure
   - entry points
   - configuration files
3. Identify modules:
   - feature modules
   - domain modules
   - shared libraries
   - infrastructure modules
   - generated code
4. Understand business workflows:
   - actors and roles
   - end-to-end flows
   - business rules
   - validation and approval steps
   - exception paths
5. Identify frontend screens and navigation:
   - routes
   - pages
   - forms
   - shared components
   - state management
   - API calls
6. Identify backend APIs and services:
   - controllers, routes, handlers, endpoints
   - service classes and business logic
   - request and response DTOs
   - validation
   - error handling
7. Analyze database schema:
   - tables, views, collections, documents, or objects
   - relationships and constraints
   - indexes
   - migrations
   - stored procedures, functions, triggers
8. Identify third-party integrations:
   - REST, SOAP, GraphQL, gRPC, events, queues, files
   - authentication method
   - retry and failure handling
   - data ownership
9. Identify batch jobs or scheduled tasks:
   - cron jobs
   - queue workers
   - background processors
   - ETL jobs
   - report generation
10. Capture security/authentication flow:
    - identity provider
    - login/logout
    - tokens, sessions, cookies
    - roles, permissions, policies
    - secrets and certificates
11. Capture deployment process:
    - build commands
    - artifact packaging
    - containers
    - infrastructure
    - environments
    - release steps
12. Prepare As-Is Architecture Document.
13. Prepare gaps, risks, and modernization opportunities.

## Questions To Ask When Context Is Missing

Ask only what is needed to continue:

- What is the application name, domain, and primary business purpose?
- Where are the source code, database scripts, deployment scripts, and documents located?
- Which environments exist today: local, dev, QA, UAT, staging, production?
- Are there known critical workflows or screens that must be analyzed first?
- Are there external systems, vendors, or compliance requirements that are not visible in code?
- Should the output be a quick inventory, standard documentation, or detailed architecture package?

## Output Format

Use this structure for the As-Is Architecture Document:

```markdown
# As-Is Architecture Document

## Executive Summary
## Source Inputs Reviewed
## Application Overview
## Technology Stack
## Module Inventory
## Business Workflows
## Frontend Screens and Navigation
## Backend APIs and Services
## Database Schema
## Integrations
## Batch Jobs and Scheduled Tasks
## Security and Authentication Flow
## Deployment Process
## Observability and Operations
## Known Gaps
## Risks
## Modernization Opportunities
## Open Questions
```

## Rules

- Distinguish evidence from assumptions.
- Include source file references when possible.
- Do not invent business rules or hidden integrations.
- Flag unknowns as open questions.
- Keep recommendations separate from current-state facts.
- Prefer diagrams for architecture, data flow, and deployment views when useful.

