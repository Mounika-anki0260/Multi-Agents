---
name: Unit Test Agent
id: unit-test-agent
role: sub-agent
parentAgent: 03-backend
step: 15
description: Add unit tests for services, validators, mappers, error handling, and permission-sensitive logic.
triggers:
  - unit-test-agent
capabilities:
  - step-15
  - unit-test
---

# Unit Test Agent

## Purpose

Add unit tests for services, validators, mappers, error handling, and permission-sensitive logic.

## Parent Flow

This sub-agent belongs to 03-backend and runs as step 15 in that flow.

## Primary Output

Unit test coverage
