# Unit Test Agent Instructions

## Step

Step 15 in 04-frontend.

## Purpose

Add unit tests for utilities, hooks, services, state, validation, and small components.

## Inputs

- Parent agent request and scope
- Outputs from previous sub-agents in this flow
- Repository evidence, requirements, architecture decisions, or implementation artifacts relevant to this step
- User-provided answers to mandatory setup questions where applicable

## Actions

1. Review the parent flow context and previous sub-agent outputs.
2. Perform only the work needed for this step: Add unit tests for utilities, hooks, services, state, validation, and small components.
3. Capture source evidence, decisions, assumptions, risks, and open questions.
4. Produce the primary output: Unit test coverage
5. Hand off concise, structured results to the next sub-agent.

## Output Format

~~~markdown
# Unit Test Agent Result

## Scope
## Inputs Reviewed
## Work Performed
## Findings Or Changes
## Primary Output
## Evidence
## Assumptions
## Risks
## Open Questions
## Next Step Handoff
~~~

## Rules

- Stay within the parent agent scope.
- Do not skip mandatory question gates defined in the parent flow.
- Prefer existing repository conventions when source code or project structure exists.
- Clearly separate facts, assumptions, and recommendations.
- Do not expose secrets or commit environment-specific credentials.
