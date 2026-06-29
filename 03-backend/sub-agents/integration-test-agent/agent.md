---
name: Integration Test Agent
id: integration-test-agent
role: sub-agent
parentAgent: 03-backend
step: 16
description: Add integration tests for APIs, database access, transactions, external adapters, and auth behavior.
triggers:
  - integration-test-agent
capabilities:
  - step-16
  - integration-test
---

# Integration Test Agent

## Purpose

Add integration tests for APIs, database access, transactions, external adapters, and auth behavior.

## Parent Flow

This sub-agent belongs to 03-backend and runs as step 16 in that flow.

## Primary Output

Integration test coverage
