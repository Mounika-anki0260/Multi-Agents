# QA Sub-Agents

These sub-agents execute QA validation step by step. The main QA Agent must ask testing setup questions before creating scripts, choosing tools, or finalizing test strategy.

## Step-by-Step Sub-Agent Flow

| Step | Sub-Agent | Purpose | Primary Output |
|---|---|---|---|
| 1 | `qa-setup-questionnaire-agent` | Ask testing scope, tools, script structure, environments, test data, entry/exit criteria, devices, defect process, performance targets, and sign-off evidence. | QA setup decisions |
| 2 | `requirements-analysis-agent` | Understand requirements, user stories, acceptance criteria, NFRs, risks, and release scope. | Requirement-to-test traceability |
| 3 | `test-strategy-agent` | Prepare overall test strategy, scope, types, tools, environments, roles, entry criteria, exit criteria, and schedule. | Test strategy |
| 4 | `test-scenario-agent` | Prepare end-to-end scenarios by feature, role, API, workflow, integration, and risk area. | Test scenarios |
| 5 | `test-case-agent` | Prepare positive, negative, boundary, role-based, validation, integration, and regression test cases. | Test case catalog |
| 6 | `test-data-agent` | Prepare test data plan, seed data, generated data, masked data, cleanup, and data ownership. | Test data plan |
| 7 | `test-environment-agent` | Verify environment availability, URLs, credentials, configuration, services, data, monitoring, and deployment version. | Test environment readiness |
| 8 | `functional-testing-agent` | Execute functional tests against requirements and acceptance criteria. | Functional test results |
| 9 | `api-testing-agent` | Execute API tests for contracts, status codes, payloads, errors, auth, pagination, filtering, and integration behavior. | API test results |
| 10 | `frontend-ui-testing-agent` | Execute UI tests for screens, navigation, forms, errors, loading, accessibility basics, and browser behavior. | UI test results |
| 11 | `integration-testing-agent` | Execute integration tests across frontend, backend, database, external systems, queues, files, and batch jobs. | Integration test results |
| 12 | `regression-testing-agent` | Execute regression suite for impacted and high-risk existing behavior. | Regression test results |
| 13 | `smoke-testing-agent` | Execute smoke checks after deployment or build promotion. | Smoke test results |
| 14 | `negative-testing-agent` | Execute invalid input, unauthorized access, boundary, failure, timeout, and error-path tests. | Negative test results |
| 15 | `performance-testing-agent` | Execute performance tests where required for response time, throughput, concurrency, error rate, and resource usage. | Performance test results |
| 16 | `defect-logging-agent` | Log defects with reproduction steps, expected result, actual result, evidence, severity, priority, environment, and owner. | Defect report |
| 17 | `fix-retest-agent` | Retest fixed defects, verify regression impact, and update defect status. | Retest report |
| 18 | `qa-report-agent` | Prepare execution summary, coverage, defects, risks, skipped tests, evidence, and residual risk. | QA report |
| 19 | `qa-signoff-agent` | Provide go/no-go recommendation based on exit criteria, open defects, risk acceptance, and approval evidence. | QA sign-off |

## Mandatory QA Question Gate

The `qa-setup-questionnaire-agent` must ask:

- Which test types are required?
- Which testing tools should be used?
- How should test scripts be structured?
- Which environments, browsers, devices, and test data are available?
- What entry, exit, defect, performance, and sign-off criteria apply?

## Handoff Rules

- Every test case should trace to a requirement, risk, API contract, or screen.
- Critical and blocker defects must prevent sign-off unless explicitly accepted.
- Production tests must be smoke-only unless explicitly approved.
- Skipped tests and residual risks must be documented.

