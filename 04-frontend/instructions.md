# Frontend Agent Instructions

## Mandatory Frontend Setup Questions

Before creating frontend layers or scaffolding a new frontend project, ask:

1. What frontend technology and version should be used?
   - React
   - Angular
   - Vue
   - Next.js
   - Svelte
   - plain HTML/CSS/JavaScript
   - other
2. How should the project structure look?
   - feature-based
   - route-based
   - atomic design
   - layered components
   - domain modules
   - existing repository pattern
3. What routing approach is required?
   - file-based routing
   - declarative route config
   - protected routes
   - nested layouts
4. What UI library or design system should be used?
   - existing design system
   - Material UI
   - Ant Design
   - Bootstrap
   - Tailwind with component library
   - custom components
5. What state management approach is expected?
   - framework state
   - Redux
   - Zustand
   - NgRx
   - Pinia
   - server-state library
6. How should APIs be integrated?
   - generated client from OpenAPI
   - handwritten client
   - GraphQL client
   - typed fetch/axios service
7. What form validation and error display pattern should be used?
8. What accessibility standard is required?
   - WCAG 2.1 AA
   - WCAG 2.2 AA
   - organization standard
9. What testing tools should be used?
   - Jest
   - Vitest
   - React Testing Library
   - Angular Testing Library
   - Cypress
   - Playwright
   - Storybook tests
10. Should the agent create a new project, extend an existing project, or only prepare design/docs?

If the repository already has a frontend convention, prefer it and ask only about missing decisions.

## Implementation Workflow

1. Read frontend architecture, screen map, API contracts, and existing code.
2. Confirm frontend setup answers.
3. Create or update frontend project setup.
4. Define project structure.
5. Configure routing and protected navigation.
6. Create app shell, layout, navigation, and shared components.
7. Set up UI library or design system.
8. Create pages/screens.
9. Create reusable components.
10. Set up state management.
11. Integrate backend APIs.
12. Add form validation.
13. Add error handling and empty states.
14. Add loading states.
15. Add accessibility checks.
16. Add unit tests.
17. Add UI/component tests.
18. Configure ESLint and Prettier.
19. Run build, tests, linting, and quality checks.
20. Fix SonarQube issues.
21. Prepare PR summary, test evidence, screenshots where useful, and review notes.

## Output Format For Frontend Notes

```markdown
# Frontend Implementation Notes

## Scope
## Project Structure
## Routing
## Layout and Shared Components
## UI Library / Design System
## Pages and Screens
## Reusable Components
## State Management
## API Integration
## Forms and Validation
## Error and Loading States
## Accessibility
## Tests Added
## Quality Checks
## SonarQube Issues Fixed
## Pull Request Checklist
## Open Questions
```

## Rules

- Prefer existing project conventions.
- Keep API logic out of visual components when a service layer exists.
- Do not hardcode secrets or environment-specific URLs.
- Include loading, empty, error, success, and unauthorized states.
- Make navigation and forms keyboard accessible.
- Add tests for rendering, user interaction, validation, API failure, and permission-sensitive states.
- Document any skipped tests or quality checks.

