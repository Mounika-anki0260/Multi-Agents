# Software Modernization Multi-Agent System

This directory defines eight reusable agents for end-to-end application modernization work. The agents are intentionally technology-agnostic so they can support monolith, modular monolith, microservices, event-driven, serverless, cloud-native, hybrid, and phased migration approaches.

## Quick Start

Use the agent that matches the workstream:

```text
@reverse-engineering-documents: Understand the existing application and prepare As-Is architecture documentation.
@legacy-specific-modernization: Create a platform-specific modernization path for COBOL, VB6, Oracle Forms, PowerBuilder, .NET Framework, Java EE/Struts, database-heavy, or batch/reporting legacy systems.
@redesign-rearchitecture-documents: Define the target system and prepare To-Be architecture documentation.
@backend: Build backend services, APIs, tests, and quality fixes.
@frontend: Build UI screens, client logic, tests, and quality fixes.
@qa: Prepare and execute quality validation across functional, API, UI, integration, regression, smoke, negative, and performance testing.
@sonarqube-code-quality: Configure and operate SonarQube quality gates and issue remediation.
@cicd-pipeline: Automate build, test, scan, artifact, deployment, smoke test, rollback, and notifications.
```

## Agents

| Agent | Purpose | Folder |
|---|---|---|
| Reverse Engineering Documents Agent | Understand the existing system and produce As-Is documentation | `01-reverse-engineering-documents` |
| Legacy-Specific Modernization Agent | Create technology-specific modernization assessment, options, and handoff roadmap | `08-legacy-specific-modernization` |
| Re-design / Re-architecture Documents Agent | Define the target system and produce To-Be documentation | `02-redesign-rearchitecture-documents` |
| Backend Agent | Build backend services and APIs | `03-backend` |
| Frontend Agent | Build user interface and client-side logic | `04-frontend` |
| QA Agent | Validate application quality | `05-qa` |
| SonarQube / Code Quality Agent | Maintain code quality and security standards | `06-sonarqube-code-quality` |
| CI/CD Pipeline Agent | Automate build, test, scan, and deployment | `07-cicd-pipeline` |

## Standard Agent Contract

Each agent folder contains:

```text
agent.md          Agent identity, purpose, triggers, and capabilities
instructions.md   Detailed operating workflow, required questions, outputs, and guardrails
prompt.md         Reusable prompt for invoking the agent directly
sub-agents/       Step-by-step specialist sub-agent workflow for that folder
` 

Each `sub-agents/README.md` defines the ordered sub-agent sequence, each sub-agent's purpose, primary output, mandatory setup question gates, and handoff rules. Each listed sub-agent also has its own folder containing `agent.md`, `instructions.md`, and `prompt.md`.

## Recommended Workflow

1. Run `@reverse-engineering-documents` to create As-Is understanding.
2. Run `@legacy-specific-modernization` when the system uses a particular legacy technology that needs focused migration guidance.
3. Run `@redesign-rearchitecture-documents` to ask target architecture questions and prepare To-Be architecture.
4. Run `@backend` and `@frontend` for implementation workstreams.
5. Run `@qa` continuously against requirements and completed features.
6. Run `@sonarqube-code-quality` on every pull request and before release gates.
7. Run `@cicd-pipeline` to automate delivery across environments.

## Decision Gates

Agents must ask clarifying setup questions before producing irreversible architecture, project structure, testing strategy, quality gate, or deployment recommendations. If answers are unavailable, the agent should document assumptions, risks, and options instead of blocking unnecessarily.

## Output Locations

Recommended output folders:

```text
docs/reverse-engineering/
docs/legacy-modernization/
docs/architecture/
docs/backend/
docs/frontend/
docs/qa/
docs/code-quality/
docs/cicd/
```

Generated code, tests, infrastructure, or pipeline files should follow the target repository's existing structure when one exists. For new projects, the responsible agent must ask structure questions before scaffolding.


