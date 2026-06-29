# Agent Index

| ID | Name | Type | Main Invocation |
|---|---|---|---|
| `reverse-engineering-documents` | Reverse Engineering Documents Agent | Discovery / Documentation | `@reverse-engineering-documents` |
| `legacy-specific-modernization` | Legacy-Specific Modernization Agent | Legacy Platform Modernization | `@legacy-specific-modernization` |
| `redesign-rearchitecture-documents` | Re-design / Re-architecture Documents Agent | Architecture / Documentation | `@redesign-rearchitecture-documents` |
| `backend` | Backend Agent | Implementation | `@backend` |
| `frontend` | Frontend Agent | Implementation | `@frontend` |
| `qa` | QA Agent | Validation | `@qa` |
| `sonarqube-code-quality` | SonarQube / Code Quality Agent | Quality Governance | `@sonarqube-code-quality` |
| `cicd-pipeline` | CI/CD Pipeline Agent | Delivery Automation | `@cicd-pipeline` |

## Sub-Agent Index

| Main Agent | Sub-Agent Workflow |
|---|---|
| `reverse-engineering-documents` | `01-reverse-engineering-documents/sub-agents/README.md` |
| `legacy-specific-modernization` | `08-legacy-specific-modernization/sub-agents/README.md` |
| `redesign-rearchitecture-documents` | `02-redesign-rearchitecture-documents/sub-agents/README.md` |
| `backend` | `03-backend/sub-agents/README.md` |
| `frontend` | `04-frontend/sub-agents/README.md` |
| `qa` | `05-qa/sub-agents/README.md` |
| `sonarqube-code-quality` | `06-sonarqube-code-quality/sub-agents/README.md` |
| `cicd-pipeline` | `07-cicd-pipeline/sub-agents/README.md` |

## Cross-Agent Handoffs

| From | To | Handoff Content |
|---|---|---|
| Reverse Engineering | Legacy-Specific Modernization | As-Is findings, artifact inventory, codebase evidence, data model, integrations, deployment notes |
| Reverse Engineering | Re-architecture | As-Is architecture, risks, gaps, integrations, deployment, data model, workflows |
| Legacy-Specific Modernization | Re-architecture | Legacy platform constraints, migration options, component mapping, compatibility risks, roadmap |
| Re-architecture | Backend | Backend architecture, API contracts, data design, auth model, NFRs |
| Re-architecture | Frontend | Frontend architecture, screen map, navigation, UX constraints, API contracts |
| Backend / Frontend | QA | Requirements, acceptance criteria, deployed build, test data, known risks |
| Backend / Frontend | SonarQube | Source code, test coverage reports, quality standards |
| SonarQube | Backend / Frontend | Issues, quality gate result, remediation assignments |
| Backend / Frontend / QA / SonarQube | CI/CD | Build commands, test commands, scan commands, deployment targets |

## Required Setup Questions By Agent

| Agent | Must Ask Before |
|---|---|
| Legacy-Specific Modernization | Selecting a platform-specific migration path or roadmap |
| Re-design / Re-architecture | Selecting architecture style and final To-Be architecture |
| Backend | Creating backend folder/package/layer structure |
| Frontend | Creating frontend folder/routing/component/state structure |
| QA | Creating test scripts, choosing tools, or defining sign-off strategy |
| SonarQube | Setting thresholds, quality gates, and severity rules |
| CI/CD | Creating deployment pipeline and environment promotion model |