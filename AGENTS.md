# Agents Overview

## 01. Reverse Engineering Documents Agent

Use `@reverse-engineering-documents` when the goal is to understand an existing application. It collects available documents, scans the codebase, identifies modules, maps frontend screens, backend APIs, database schema, integrations, batch jobs, security flows, deployment process, risks, and modernization opportunities.

Primary outputs:

- As-Is Architecture Document
- Current-state module inventory
- Business workflow map
- API, data, integration, security, batch, and deployment summaries
- Gap, risk, and modernization opportunity report

## 02. Re-design / Re-architecture Documents Agent

Use `@redesign-rearchitecture-documents` when the goal is to define the target system. It asks architecture setup questions first, then designs the target architecture, technology stack, layers, frontend, backend, database, API contracts, auth model, observability, scalability, migration, deployment, review comments, and approvals.

Primary outputs:

- To-Be Architecture Document
- Architecture decision log
- Migration strategy
- Review comments and approval checklist

## 03. Backend Agent

Use `@backend` when backend code or backend design is needed. It asks backend structure questions before scaffolding, then sets up project structure, profiles, database connectivity, models, repositories, services, controllers, DTOs, validation, auth, exception handling, logging, tests, code quality fixes, and pull request readiness.

Primary outputs:

- Backend source changes
- API implementation and tests
- Backend design notes
- PR checklist and code quality report

## 04. Frontend Agent

Use `@frontend` when UI screens or client-side logic are needed. It asks frontend structure questions before scaffolding, then configures routing, layout, shared components, UI library, pages, reusable components, state management, API integration, validation, errors, loading states, accessibility, tests, linting, formatting, and PR readiness.

Primary outputs:

- Frontend source changes
- Page and component implementation
- Accessibility and testing notes
- PR checklist and code quality report

## 05. QA Agent

Use `@qa` when quality validation is needed. It asks testing setup questions before creating scripts or test plans, then prepares strategy, scenarios, cases, data, environment, functional, API, UI, integration, regression, smoke, negative, and performance testing, logs defects, retests fixes, prepares QA reports, and gives sign-off.

Primary outputs:

- Test strategy
- Test scenarios and cases
- Defect report
- QA execution report and sign-off

## 06. SonarQube / Code Quality Agent

Use `@sonarqube-code-quality` when static analysis and quality gates are needed. It configures SonarQube projects, scanners, quality gates, coverage thresholds, code smell, vulnerability, duplicate-code checks, CI/CD integration, pull request scans, quality reports, issue assignment, blocker and critical remediation, re-scans, and approval checks.

Primary outputs:

- SonarQube configuration
- Quality gate definition
- Scan reports
- Remediation plan and gate approval status

## 07. CI/CD Pipeline Agent

Use `@cicd-pipeline` when delivery automation is needed. It defines stages, checkout, dependency install, build, tests, SonarQube, security scans, artifacts, Docker images, registry push, dev and QA/UAT deployment, production approval gate, production deployment, post-deployment smoke tests, rollback, and notifications.

Primary outputs:

- Pipeline configuration
- Deployment automation
- Rollback plan
- Release verification report

## 08. Legacy-Specific Modernization Agent

Use `@legacy-specific-modernization` when the legacy system belongs to a particular technology family that needs targeted migration guidance, such as Mainframe COBOL, VB6/COM, Oracle Forms/Reports, PowerBuilder, .NET Framework, Java EE/Struts, database-heavy stored procedure applications, or legacy batch/reporting workloads.

Primary outputs:

- Legacy modernization intake
- Platform-specific assessment
- Artifact inventory
- Modernization options and recommended path
- Component mapping and phased roadmap
- Handoff checklist for architecture, implementation, QA, quality, and CI/CD

## Sub-Agent Workflows

| Main Agent | Sub-Agent Folder | Sub-Agent Count |
|---|---|---:|
| `reverse-engineering-documents` | `01-reverse-engineering-documents/sub-agents/` | 13 |
| `redesign-rearchitecture-documents` | `02-redesign-rearchitecture-documents/sub-agents/` | 16 |
| `backend` | `03-backend/sub-agents/` | 20 |
| `frontend` | `04-frontend/sub-agents/` | 21 |
| `qa` | `05-qa/sub-agents/` | 19 |
| `sonarqube-code-quality` | `06-sonarqube-code-quality/sub-agents/` | 15 |
| `cicd-pipeline` | `07-cicd-pipeline/sub-agents/` | 19 |
| `legacy-specific-modernization` | `08-legacy-specific-modernization/sub-agents/` | 10 |
