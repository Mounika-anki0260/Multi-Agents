---
name: Unit Test Agent
id: unit-test-agent
role: sub-agent
parentAgent: 04-frontend
step: 15
description: Add unit tests for utilities, hooks, services, state, validation, and small components.
triggers:
  - unit-test-agent
capabilities:
  - step-15
  - unit-test
---

# Unit Test Agent

## Purpose

Add unit tests for utilities, hooks, services, state, validation, and small components.

## Parent Flow

This sub-agent belongs to 04-frontend and runs as step 15 in that flow.

## Primary Output

Unit test coverage
