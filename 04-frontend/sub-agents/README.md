# Frontend Sub-Agents

These sub-agents execute frontend delivery step by step. The main Frontend Agent must ask structure, routing, UI, state, API, validation, accessibility, and test questions before scaffolding.

## Step-by-Step Sub-Agent Flow

| Step | Sub-Agent | Purpose | Primary Output |
|---|---|---|---|
| 1 | `frontend-setup-questionnaire-agent` | Ask frontend stack, version, project structure, routing, UI library, state management, API integration, validation, accessibility, and test tools. | Frontend setup decisions |
| 2 | `frontend-project-setup-agent` | Create or validate frontend project setup, dependency manager, build tool, scripts, environment handling, and developer commands. | Frontend project baseline |
| 3 | `project-structure-agent` | Define feature-based, route-based, atomic, domain-based, layered, or existing project structure. | Frontend structure map |
| 4 | `routing-agent` | Configure routes, nested layouts, protected routes, redirects, route metadata, and navigation guards. | Routing setup |
| 5 | `layout-shared-components-agent` | Set up app shell, navigation, layout, headers, sidebars, footers, modals, toasts, and shared primitives. | Layout and shared components |
| 6 | `ui-library-design-system-agent` | Configure UI library, theme tokens, typography, spacing, icons, forms, tables, accessibility defaults, and design standards. | UI system setup |
| 7 | `page-screen-agent` | Create pages/screens aligned to user journeys, requirements, and API contracts. | Page and screen implementation |
| 8 | `reusable-component-agent` | Create reusable components for fields, tables, cards, dialogs, filters, actions, empty states, and error displays. | Component library |
| 9 | `state-management-agent` | Set up client state, server state, caching, invalidation, selectors, stores, and persistence where needed. | State management setup |
| 10 | `backend-api-integration-agent` | Integrate backend APIs using generated clients, typed services, GraphQL clients, fetch/axios wrappers, or existing API patterns. | API integration layer |
| 11 | `form-validation-agent` | Add form state, validation rules, error messages, touched/dirty states, submit handling, and disabled states. | Form validation |
| 12 | `error-handling-agent` | Add API error handling, unauthorized states, not-found states, empty states, retry options, and user-friendly messages. | Error state coverage |
| 13 | `loading-states-agent` | Add loading, skeleton, progress, optimistic update, disabled action, and pending submission states. | Loading state coverage |
| 14 | `accessibility-agent` | Check keyboard navigation, focus management, semantic HTML, labels, ARIA where needed, color contrast, and screen reader behavior. | Accessibility findings and fixes |
| 15 | `unit-test-agent` | Add unit tests for utilities, hooks, services, state, validation, and small components. | Unit test coverage |
| 16 | `ui-component-test-agent` | Add component and UI tests for rendering, interaction, validation, loading, error, and permission states. | UI/component test coverage |
| 17 | `eslint-prettier-agent` | Configure ESLint, Prettier, formatting scripts, lint rules, import rules, and repo-specific style standards. | Lint and format setup |
| 18 | `code-quality-agent` | Run build, tests, linting, formatting, static analysis, and coverage checks. | Code quality result |
| 19 | `sonarqube-fix-agent` | Fix SonarQube blocker, critical, vulnerability, duplication, and code smell issues. | SonarQube remediation |
| 20 | `pull-request-agent` | Prepare PR summary, test evidence, accessibility notes, screenshots where useful, and review checklist. | Pull request readiness |
| 21 | `code-review-merge-agent` | Support review comments, update code, rerun checks, and confirm merge readiness. | Merge readiness status |

## Mandatory Frontend Question Gate

The `frontend-setup-questionnaire-agent` must ask:

- What frontend stack and version should be used?
- How should the project structure look?
- What routing, UI library, state management, and API integration approaches are expected?
- What validation, accessibility, browser support, and testing standards apply?
- Should this create a new project, extend an existing project, or only document the frontend design?

## Handoff Rules

- Screen and navigation decisions must be recorded before page creation.
- API integration must reference approved API contracts.
- Accessibility must be checked before PR readiness.
- Environment-specific URLs and secrets must stay outside source control.

